
SUBDIRS = . tests

dist_pkgdata_DATA =				\
		${srcdir}/README		\
		${srcdir}/*.[ch]		\
		${srcdir}/file-dependencies

smodsdir=$(pkgdata)

nobase_dist_smods_DATA =     \
	standard-modules/README  \
	standard-modules/ASN1-Object-Identifier-Module.asn1 \
	standard-modules/ASN1C-UsefulInformationObjectClasses.asn1


uninstall-local:
	-@echo -n " "
	-rm -f -r $(DESTDIR)$(pkgdatadir)

check_LTLIBRARIES = libasn1cskeletons.la

libasn1cskeletons_la_CFLAGS = $(TESTSUITE_CFLAGS)
libasn1cskeletons_la_SOURCES = 				\
	ANY.c ANY.h					\
	BIT_STRING.c BIT_STRING.h			\
	BMPString.c BMPString.h				\
	BOOLEAN.c BOOLEAN.h				\
	ENUMERATED.c ENUMERATED.h			\
	GeneralString.c GeneralString.h			\
	GeneralizedTime.c GeneralizedTime.h		\
	GraphicString.c GraphicString.h			\
	IA5String.c IA5String.h				\
	INTEGER.c INTEGER.h				\
	ISO646String.c ISO646String.h			\
	NULL.c NULL.h					\
	NativeEnumerated.c NativeEnumerated.h		\
	NativeInteger.c NativeInteger.h			\
	NativeReal.c NativeReal.h			\
	NumericString.c NumericString.h			\
	OBJECT_IDENTIFIER.c OBJECT_IDENTIFIER.h		\
	OCTET_STRING.c OCTET_STRING.h			\
	ObjectDescriptor.c ObjectDescriptor.h		\
	PrintableString.c PrintableString.h		\
	REAL.c REAL.h					\
	RELATIVE-OID.c RELATIVE-OID.h			\
	T61String.c T61String.h				\
	TeletexString.c TeletexString.h			\
	UTCTime.c UTCTime.h				\
	UTF8String.c UTF8String.h			\
	UniversalString.c UniversalString.h		\
	VideotexString.c VideotexString.h		\
	VisibleString.c VisibleString.h			\
	asn_SEQUENCE_OF.c asn_SEQUENCE_OF.h		\
	asn_SET_OF.c asn_SET_OF.h			\
	asn_application.h asn_codecs.h			\
	asn_codecs_prim.c asn_codecs_prim.h		\
	asn_internal.h asn_system.h			\
	ber_decoder.c ber_decoder.h			\
	ber_tlv_length.c ber_tlv_length.h		\
	ber_tlv_tag.c ber_tlv_tag.h			\
	constr_CHOICE.c constr_CHOICE.h			\
	constr_SEQUENCE.c constr_SEQUENCE.h		\
	constr_SEQUENCE_OF.c constr_SEQUENCE_OF.h	\
	constr_SET.c constr_SET.h			\
	constr_SET_OF.c constr_SET_OF.h			\
	constr_TYPE.c constr_TYPE.h			\
	constraints.c constraints.h			\
	der_encoder.c der_encoder.h			\
	per_decoder.c per_decoder.h			\
	per_encoder.c per_encoder.h			\
	per_opentype.c per_opentype.h			\
	per_support.c per_support.h			\
	xer_decoder.c xer_decoder.h			\
	xer_encoder.c xer_encoder.h			\
	xer_support.c xer_support.h

