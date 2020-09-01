# oatpp-nixos-feed
Oat++ patches for NixOS


cmakelibsdir.patch

This patch fixes an issue in a Nix environment (OS or shell) where the variable
@OATPP_MODULE_LIBDIR@ was being substitued with an erroneous path. Any project
using Cmake FindPackage to locate oatpp would get back a bad path contained
in oatpp_LIBRARIES_DIRS.
