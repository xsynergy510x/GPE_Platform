How to build Module for Platform
- It is only for modules are needed to using Android build system.
- Please check its own install information under its folder for other module.

[Step to build]
1. Get android open source.
	: version info - Android 5.1.0_r5
	( Download site : http://source.android.com )

2. Copy module that you want to build to original android open source. If same module exist in android open source, you should replace it. (no overwrite)
	# It is possible to build all modules at once.

3. You should add module name to 'PRODUCT_PACKAGES' in 'build\target\product\core.mk' as following case.
	case 1) e2fsprog : should add 'e2fsck' to PRODUCT_PACKAGES	
	case 2) libexifa : should add 'libexifa' to PRODUCT_PACKAGES
	case 3) libjpega : should add 'libjpega' to PRODUCT_PACKAGES	

4. excute build command
	./build.sh user
