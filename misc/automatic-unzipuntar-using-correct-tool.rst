Automatic unzip/untar using correct tool
========================================================================================================

.. sectionauthor:: Martin Fitzpatrick <martin.fitzpatrick@gmail.com>
.. tags:: unzip,tar,uncompress

An alias for bash profile to automatically unzip/untar compressed files using the correct tool, without needing to know the syntax.








- Add the following to your `.bashrc` or `.profile` file:

	extract () {
    if [ -f $1 ] ; then
        case $1 in
            *.tar.bz2)  tar xjf $1      ;;
            *.tar.gz)   tar xzf $1      ;;
            *.bz2)      bunzip2 $1      ;;
            *.rar)      rar x $1        ;;
            *.gz)       gunzip $1       ;;
            *.tar)      tar xf $1       ;;
            *.tbz2)     tar xjf $1      ;;
            *.tgz)      tar xzf $1      ;;
            *.zip)      unzip $1        ;;
            *.Z)        uncompress $1   ;;
            *)          echo "'$1' cannot be extracted via extract()" ;;
        esac
    else
        echo "'$1' is not a valid file"
    fi
    }



- From the prompt compress any file with `extract <filename>`






    This method is based, with permission, on an original protocol available 
    `here <(http://unix.stackexchange.com/a/168>`__.

