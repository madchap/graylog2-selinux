Based on info at https://selinuxproject.org/page/NB_AL

Tested with grokdebug.herokuapp.com with examples given in above link. I am currently lacking actual true values for fields.

Note: when copying/pasting examples to test, mind the newlines; it has to be a single line.

Examples, if the above link is to vanish:

```type=AVC msg=audit(1239116352.727:311): avc: granted { transition } for pid=7687 comm="bash" path="/usr/move_file/move_file_c" dev=dm-0 ino=402139 scontext=unconfined_u:unconfined_r:unconfined_t tcontext=unconfined_u:unconfined_r:move_file_t tclass=process```

```type=AVC msg=audit(1242575005.122:101): avc: denied { rename } for pid=2508 comm="canberra-gtk-pl" name="c73a516004b572d8c845c74c49b2511d:runtime.tmp" dev=dm-0 ino=188999 scontext=test_u:staff_r:oddjob_mkhomedir_t:s0 tcontext=test_u:object_r:gnome_home_t:s0 tclass=lnk_file```

```type=AVC msg=audit(1242575005.122:101): avc: denied { unlink } for pid=2508 comm="canberra-gtk-pl" name="c73a516004b572d8c845c74c49b2511d:runtime"
dev=dm-0 ino=188578 scontext=test_u:staff_r:oddjob_mkhomedir_t:s0 tcontext=system_u:object_r:gnome_home_t:s0 tclass=lnk_file```

