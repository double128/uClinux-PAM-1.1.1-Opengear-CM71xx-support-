The main difference between `pam_adduser.c` and `pam_adduser-MODIFIED.c` is that the latter is edited to remove specific functionality that prevents a remotely-authenticated (in my case, RADIUS) user from being in more than one local group at a time. This functionality was needed for the device I am working on. If this kind of functionality sounds good to you, then you are free to use it. Just keep in mind that the code is poorly modified, but it still works as intended.

If you intend on using my modified version of the code, then don't forget to rename `pam_adduser-MODIFIED.c` to just `pam_adduser.c`

NOTE: The .so file that's uploaded here is the modified version of the PAM module.
