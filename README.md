# uDemo_Hydra
Add the following to .git/config at the bottom

  `[alias]  `
  
  `sbu = "!f() { git subtree pull --prefix $2 $1 master --squash; }; f"  `

	`chs = !git fetch origin master; && git pull origin ; && git subtree pull --prefix=modules\Common uDemo_Hydra_Common master;  `

	`staadd = "!f() { git subtree add --prefix=./modules/Common uDemo_Hydra_Common --squash; }; f"  `

	`stupdate="!f() { git subtree pull --prefix=./modules/Common uDemo_Hydra_Common master ; }; f"  `

	`stpush = "!f() { git subtree push --prefix=./modules/Common uDemo_Hydra_Common master ; }; f"  `
	
  `
