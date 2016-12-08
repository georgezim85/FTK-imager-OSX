# Forensics ToolKit Imager
The FTK Imager is a simple but concise tool. It saves an image of a hard disk in one file or in segments that may be later on reconstructed. It calculates MD5 hash values and confirms the integrity of the data before closing the files.

# Install FTK Imager For Mac OSX
                    git clone https://github.com/MrMugiwara/FTK-imager-OSX.git
                    cd FTK-imager-OSX
                    chmod +x ftkimager
                    ./ftkimager -h

# How To Use FTK Imager On MAC OSX

        Usage:  ./ftkimager source [dest_file] [options] 
          
        AccessData FTK Imager Copyright 2006-2012 AccessData Corp. 
        384 South 400 West, Lindon, UT 84042 All rights reserved.
                    source can specify a block device, a supported image file, or `-' for stdin
                    if dest_file is specified, proper extension for image type will be appended
                    if dest_file is `-' or not specified, raw data will be written to stdout
                    Options:
        --help        : display this information
        --list-drives : show detected physical drives
        --verify      : hash/verify the destination image,
                  or the source image if no destination is specified
        --print-info  : print information about a drive or image and then exit
        --quiet       : do not show create/verify progress information
        --no-sha1     : do not compute SHA1 hash during acquire or verify
          (The following options are valid only when dest_file is specified):
        --s01         : create a SMART ew-compressed image
        --e01         : create an E01 format image
        --frag x{K|M|G|T} : create image fragments at most x {K|M|G|T} in size
                  also accepts kB, MB, GB, and TB for powers of 10 instead of 2
        --compress C  : set compression level to C (0=none, 1=fast, ..., 9=best)
        e01/smart metadata (use quote marks when X contains spaces):
        --case-number X
        --evidence-number X
        --description X
        --examiner X
        --notes X
        AD Encryption Options:
        --inpass P      : decrypt source file using password P
        --incert C [P]  : decrypt source file using certificate C with password P
        --outpass P     : encrypt dest file using password P
        --outcert C [P] : encrypt dest file using certificate C with password P
#Exemple :
  ![alt tag](https://github.com/MrMugiwara/FTK-imager-OSX/blob/master/ftk.png)

By Soufiane Boussali<br>
Source : AccessData<br>
 ![alt tag](https://github.com/MrMugiwara/FTK-imager-OSX/blob/master/accessdata.gif)
