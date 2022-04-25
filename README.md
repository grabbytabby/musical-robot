# musical-robot
Music_Player_NFT-Tabs Generated for SHX-Connect
toolage detailed by sticky_bot

video agent enables hologram
let holonixPath = (import ./nix/sources.nix).holonix; 

# points to the current state of the Holochain repository
  holonix = import (holonixPath) {

holochainVersionId = "v0_0_124"; # specifies the Holochain version
  };
  nixpkgs = holonix.pkgs;
in nixpkgs.mkShell {
  inputsFrom = [ holonix.main ];
 
 packages = with nixpkgs; [
    niv
    # any additional packages needed for this project, e. g. Nodejs
  ];}
