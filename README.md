# BramsModel-gnu13

Versão do modelo BRAMS 6 e Prep-chem-src 1.8.3

compilado com flags para funcionar com compilador GNU 13 

FLAGS PREP-CHEM-SRC(include.opt.gfortran): -std=legacy
FLAGS BRAMS(Make_utils.in e Makefile.in): -std=legacy e  FCFLAGS=$(FC_FLAGS) -ldl -Wl,--allow-multiple-definition

-Wl,--allow-multiple-definition - Foi adicionado por causa da biblioteca wgrib2 que estava apresentando conflito
