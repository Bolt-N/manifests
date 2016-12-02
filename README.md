##Initialize the source##
repo init -u https://github.com/Bolt-N/platform_manifest.git -b N

##Sync the source##
repo sync -jx -f (x being however many cpu jobs)

##Setup build environment##
. build/envsetup.sh

##Get the right device to build##
lunch bolt_shamu-user

##Build it##
make bolt -jx (x being however many cpu jobs)


