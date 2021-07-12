# Getting started with git submodule

## Add submodule

    git submodule add <URL repo.git> <path_to_submodule_folder>\

`Including`
 
<URL repo.git>: link git that can clone repo to computer.\
<path_to_submodule_folder>: local folder have submodule on computer.

## Update submodule

    git submodule update --init\
    git submodule update --recursive --remote\
    git pull --recurse-submodules

## Remove submodule

    git submodule deinit <path_to_submodule_folder> -f\
    git rm <path_to_submodule_folder>\
    git commit -m "Remove submodule" \
    rm -rf .git/modules/<path_to_submodule_folder>\