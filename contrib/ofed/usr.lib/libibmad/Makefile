# $FreeBSD$

SHLIBDIR?=	/usr/lib

.include <bsd.own.mk>
.include "../Makefile.inc"

IBSRCDIR=	${IBMADDIR}/src

.PATH: ${IBSRCDIR}

LIB=		ibmad
SHLIB_MAJOR=	1
MK_PROFILE=	no

SRCS=	dump.c fields.c gs.c mad.c portid.c register.c resolve.c rpc.c sa.c \
	serv.c smp.c vendor.c

LIBADD=	ibcommon ibumad
CFLAGS+= -DHAVE_CONFIG_H

VERSION_MAP= ${IBSRCDIR}/libibmad.map

.include <bsd.lib.mk>
