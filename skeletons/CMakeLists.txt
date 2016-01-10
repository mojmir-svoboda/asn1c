project(asn1c_backend)
cmake_minimum_required(VERSION 3.3)

set(ASN1_SOURCES
  asn_codecs_prim.c
  asn_SET_OF.c
  asn_SEQUENCE_OF.c
  ber_decoder.c
  ber_tlv_length.c
  ber_tlv_tag.c
  BIT_STRING.c
  constr_CHOICE.c
  constr_SEQUENCE.c
  constr_SEQUENCE_OF.c
  constr_SET_OF.c
  constr_TYPE.c
  constraints.c
  der_encoder.c
  INTEGER.c
  NativeEnumerated.c
  NativeInteger.c
  OCTET_STRING.c
  BOOLEAN.c
  per_decoder.c
  per_encoder.c
  per_opentype.c
  per_support.c
  xer_decoder.c
  xer_encoder.c
  xer_support.c
)

set(ASN1_HEADERS
  asn_application.h
  asn_codecs.h
  asn_codecs_prim.h
  asn_internal.h
  asn_system.h
  ber_decoder.h
  ber_tlv_length.h
  ber_tlv_tag.h
  BIT_STRING.h
  constr_CHOICE.h
  constr_SEQUENCE.h
  constr_TYPE.h
  constraints.h
  der_encoder.h
  INTEGER.h
  NativeEnumerated.h
  NativeInteger.h
  OCTET_STRING.h
  BOOLEAN.h
  per_decoder.h
  per_encoder.h
  per_opentype.h
  per_support.h
  xer_decoder.h
  xer_encoder.h
  xer_support.h
)

include_directories(.)
add_library(asn1c_backend STATIC ${ASN1_SOURCES})
set_source_files_properties(${ASN1_SOURCES} PROPERTIES LANGUAGE CXX)
set_target_properties(asn1c_backend PROPERTIES LINKER_LANGUAGE CXX)

