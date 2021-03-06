
BUILT_SOURCES= \
	parser/seclang-parser.cc

lib_LTLIBRARIES = libmodsecurity.la
libmodsecurity_ladir = $(prefix)/include
libmodsecurity_includesub_collectiondir = $(pkgincludedir)/collection/
libmodsecurity_includesub_actionsdir = $(pkgincludedir)/actions/

CLEANFILES = \
	location.hh \
	position.hh \
	parser/seclang-parser.cc \
	parser/seclang-parser.hh \
	parser/seclang-scanner.cc \
	stack.hh

EXTRA_DIST = $(CLEANFILES)

MAINTAINERCLEANFILES = \
	Makefile.in \
	config.h.in \
	config.h.in~


pkginclude_HEADERS = \
	../headers/modsecurity/transaction.h \
	../headers/modsecurity/debug_log.h \
	../headers/modsecurity/audit_log.h \
	../headers/modsecurity/intervention.h \
	../headers/modsecurity/modsecurity.h \
	../headers/modsecurity/rule.h \
	../headers/modsecurity/rule_message.h \
	../headers/modsecurity/rules.h \
	../headers/modsecurity/rules_properties.h \
	../headers/modsecurity/rules_exceptions.h



libmodsecurity_includesub_collection_HEADERS = \
	../headers/modsecurity/collection/collection.h \
	../headers/modsecurity/collection/collections.h \
	../headers/modsecurity/collection/variable.h


libmodsecurity_includesub_actions_HEADERS = \
	../headers/modsecurity/actions/action.h


noinst_HEADERS = \
	actions/*.h \
	actions/ctl/*.h \
	actions/data/*.h \
	actions/disruptive/*.h \
	actions/transformations/*.h \
	debug_log/*.h \
	audit_log/writer/*.h \
	collection/backend/*.h \
	operators/*.h \
	parser/*.h \
	request_body_processor/*.h \
	utils/*.h \
	variables/*.h \
	variables/variations/*.h \
	*.h


VARIABLES = \
	variables/duration.cc \
	variables/env.cc \
	variables/highest_severity.cc \
	variables/modsec_build.cc \
	variables/remote_user.cc \
	variables/time.cc \
	variables/time_day.cc \
	variables/time_epoch.cc \
	variables/time_hour.cc \
	variables/time_min.cc \
	variables/time_mon.cc \
	variables/time_sec.cc \
	variables/time_wday.cc \
	variables/time_year.cc \
	variables/tx.cc \
	variables/variable.cc \
	variables/variations/count.cc \
	variables/variations/exclusion.cc \
	variables/xml.cc \
	variables/rule.cc


ACTIONS = \
	actions/accuracy.cc \
	actions/action.cc \
	actions/audit_log.cc \
	actions/capture.cc \
	actions/chain.cc \
	actions/ctl/audit_log_parts.cc \
	actions/ctl/request_body_processor_json.cc \
	actions/ctl/request_body_processor_xml.cc \
	actions/ctl/rule_remove_target_by_tag.cc \
	actions/ctl/rule_remove_target_by_id.cc \
	actions/ctl/rule_remove_by_id.cc \
	actions/ctl/request_body_access.cc\
	actions/disruptive/allow.cc \
	actions/disruptive/block.cc \
	actions/disruptive/deny.cc \
	actions/disruptive/redirect.cc \
	actions/disruptive/pass.cc \
	actions/init_col.cc \
	actions/log.cc \
	actions/log_data.cc \
	actions/maturity.cc \
	actions/msg.cc \
	actions/multi_match.cc \
	actions/no_audit_log.cc \
	actions/no_log.cc \
	actions/phase.cc \
	actions/rev.cc \
	actions/rule_id.cc \
	actions/severity.cc \
	actions/set_sid.cc \
	actions/set_uid.cc \
	actions/set_var.cc \
	actions/data/status.cc \
	actions/skip.cc \
	actions/skip_after.cc \
	actions/tag.cc \
	actions/transformations/base64_decode.cc \
	actions/transformations/base64_encode.cc \
	actions/transformations/base64_decode_ext.cc \
	actions/transformations/cmd_line.cc \
	actions/transformations/compress_whitespace.cc \
	actions/transformations/css_decode.cc \
	actions/transformations/escape_seq_decode.cc \
	actions/transformations/hex_decode.cc \
	actions/transformations/hex_encode.cc \
	actions/transformations/html_entity_decode.cc \
	actions/transformations/js_decode.cc \
	actions/transformations/length.cc \
	actions/transformations/lower_case.cc \
	actions/transformations/md5.cc \
	actions/transformations/none.cc \
	actions/transformations/normalise_path.cc \
	actions/transformations/normalise_path_win.cc \
	actions/transformations/parity_even_7bit.cc \
	actions/transformations/parity_odd_7bit.cc \
	actions/transformations/parity_zero_7bit.cc \
	actions/transformations/remove_comments.cc \
	actions/transformations/remove_comments_char.cc \
	actions/transformations/remove_nulls.cc \
	actions/transformations/remove_whitespace.cc \
	actions/transformations/replace_comments.cc \
	actions/transformations/replace_nulls.cc \
	actions/transformations/sha1.cc \
	actions/transformations/sql_hex_decode.cc \
	actions/transformations/transformation.cc \
	actions/transformations/trim.cc \
	actions/transformations/trim_left.cc \
	actions/transformations/trim_right.cc \
	actions/transformations/url_decode.cc \
	actions/transformations/url_decode_uni.cc \
	actions/transformations/url_encode.cc \
	actions/transformations/utf8_to_unicode.cc \
	actions/ver.cc \
	actions/xmlns.cc


OPERATORS = \
	operators/begins_with.cc \
	operators/contains.cc \
	operators/contains_word.cc \
	operators/detect_sqli.cc \
	operators/detect_xss.cc \
	operators/ends_with.cc \
	operators/eq.cc \
	operators/fuzzy_hash.cc \
	operators/ge.cc \
	operators/geo_lookup.cc \
	operators/gsblookup.cc \
	operators/gt.cc \
	operators/inspect_file.cc \
	operators/ip_match.cc \
	operators/ip_match_f.cc \
	operators/ip_match_from_file.cc \
	operators/le.cc \
	operators/lt.cc \
	operators/no_match.cc \
	operators/operator.cc \
	operators/pm.cc \
	operators/pm_f.cc \
	operators/pm_from_file.cc \
	operators/rbl.cc \
	operators/rsub.cc \
	operators/rx.cc \
	operators/str_eq.cc \
	operators/str_match.cc \
	operators/validate_byte_range.cc \
	operators/validate_dtd.cc \
	operators/validate_hash.cc \
	operators/validate_schema.cc \
	operators/validate_url_encoding.cc \
	operators/validate_utf8_encoding.cc \
	operators/verify_cc.cc \
	operators/verify_cpf.cc \
	operators/verify_ssn.cc \
	operators/within.cc \
	operators/unconditional_match.cc


UTILS = \
	utils/acmp.cc \
	utils/base64.cc \
	utils/decode.cc \
	utils/geo_lookup.cc \
	utils/https_client.cc \
	utils/ip_tree.cc \
	utils/md5.cc \
	utils/msc_tree.cc \
	utils/random.cc \
	utils/regex.cc \
	utils/sha1.cc \
	utils/string.cc \
	utils/system.cc \
	utils/shared_files.cc



COLLECTION = \
	collection/collections.cc \
	collection/backend/in_memory-per_process.cc \
	collection/backend/lmdb.cc


BODY_PROCESSORS = \
	request_body_processor/multipart.cc \
	request_body_processor/xml.cc \
	request_body_processor/json.cc


libmodsecurity_la_SOURCES = \
	parser/seclang-parser.yy \
	parser/seclang-scanner.ll \
	parser/driver.cc \
	transaction.cc \
	audit_log/audit_log.cc \
	audit_log/writer/writer.cc \
	audit_log/writer/https.cc \
	audit_log/writer/serial.cc \
	audit_log/writer/parallel.cc \
	modsecurity.cc \
	rules.cc \
	debug_log/debug_log.cc \
	debug_log/debug_log_writer.cc \
	macro_expansion.cc \
	rule.cc \
	rule_message.cc \
	unique_id.cc \
	rules_exceptions.cc \
	${BODY_PROCESSORS} \
	${ACTIONS} \
	${COLLECTION} \
	${OPERATORS} \
	${UTILS} \
	${VARIABLES}


libmodsecurity_la_CFLAGS = 


libmodsecurity_la_CPPFLAGS = \
	-std=c++11 \
	-I.. \
	-g \
	-I../others \
	-fPIC \
	-O3 \
	-I../headers \
	$(GEOIP_CFLAGS) \
	$(GLOBAL_CPPFLAGS) \
	$(MODSEC_NO_LOGS) \
	$(YAJL_CFLAGS) \
	$(LMDB_CFLAGS) \
	$(PCRE_CFLAGS) \
	$(LIBXML2_CFLAGS)

libmodsecurity_la_LIBADD = \
	$(GLOBAL_LDADD) \
	$(CURL_LDADD) \
	$(GEOIP_LDFLAGS) $(GEOIP_LDADD) \
	@LEXLIB@ \
	$(PCRE_LDADD) \
	$(YAJL_LDFLAGS) $(YAJL_LDADD) \
	$(LMDB_LDFLAGS) $(LMDB_LDADD) \
	$(LIBXML2_LDADD) \
	../others/libinjection.la \
	../others/libmbedtls.la


libmodsecurity_la_LDFLAGS = \
	-version-info @MSC_VERSION_INFO@


