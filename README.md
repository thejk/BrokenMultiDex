# BrokenMultiDex
Sample project showing error in aapt

If you compile "master" branch the file "app/build/intermediates/legacy_multidex_aapt_derived_proguard_rules/debug/manifest_keep.txt" generated by aapt is empty.

If you instead switch to "fixed" branch the file now contains MainActivity and CustomProvider ensuring working MultiDex even on older Android devices. 
Fixed only adds a process name to the application, the same as the default process name.
