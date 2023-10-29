# pnix

A convenience wrapper script for NixOS operations.

    usage: pnix <command> [options]
    
       all         same as optimize + collect
       build       run "/etc/nixos/build"
       gc          run "sudo nix-collect-garbage" and "nix-collect-garbage" (as user)
       rm N        run "sudo nix-env -p /nix/var/nix/profiles/system --delete-generations N"
       rm id N     run "nix-env --delete-generations"
       du          show disk usage of generations and profiles
       list        run "sudo nix-env -p /nix/var/nix/profiles/system --list-generations"
       optimize    run "sudo nix-store --optimise"
       switch      run "/etc/nixos/build switch"
       test        run "/etc/nixos/build test"
       update      run "sudo nix-channel --update" and "nix-channel --update" (as user)
       vi|edit     run "vi /etc/nixos/$HOSTNAME/configuration.nix"

