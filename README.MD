This is a patch file for wsjt-x version 2.6.1 which adds the '-P' command
to the 'jt9' program. This feature allows for persistent storage of hash
file information between program executions. The '-P' command takes a single
argument which is the filename and path to store and retrieve
the hash information.

Typical usage: 'jt9 -P hash.dat -8 -d 3 foo.wav'

WSJT-X 2.6.1 can be obtained at https:/wsjt.sourceforge.io

To use this, you need to build the system from source. Obtain the wsjtx-2.6.1.tgz
file and build following the instructions in the INSTALL file. After the step where you
untar the file, cd into '~/build/wsjtx-2.6.1' and replace the 0 byte file
'wsjtx.patch' with the file from this repository. Then continue to build the system
as described in the INSTALL file.

Just a few notes. If you change bands or are restarting, you should remove the file
before continuing. Also, if you are using something like hermes-light with multiple
receivers, you need to make sure that each receiver is using a different hash file.