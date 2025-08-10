
# gcc90 is now the default.  See sys.mk for WORLD_ALTCOMPILER default.
#
SUBDIR+= gcc90

.if !defined(NO_ALTCOMPILER)
. if defined(WORLD_ALTCOMPILER) && (${WORLD_ALTCOMPILER} == "all" || ${WORLD_ALTCOMPILER:Mgcc80})
SUBDIR+= gcc80
. endif
.endif

SUBDIR+= libcryptsetup libdevmapper libdialog libluks liblvm
SUBDIR_ORDERED=

.include <bsd.subdir.mk>
