![TownTelecom logo](https://pbs.twimg.com/profile_images/753388670519021568/u0yjwI-k_400x400.jpg)

# Town Telecom Asterisk 16 WebRTC Boilerplate


__modules.conf:__


[modules]
autoload=yes
;
; ODBC SUPPORT
;
preload => cdr_odbc.so
preload => res_config_odbc.so
;
; VOICEMAIL SUPPORT
;
preload => res_mwi_external.so
;
; APPLICATIONS
;
;noload => app_adsiprog.so
;noload => app_agent_pool.so
;noload => app_alarmreceiver.so
;noload => app_amd.so
;noload => app_authenticate.so
;noload => app_bridgeaddchan.so
;noload => app_bridgewait.so
;noload => app_cdr.so
;noload => app_celgenuserevent.so
;noload => app_chanisavail.so
;noload => app_channelredirect.so
;noload => app_chanspy.so
;noload => app_confbridge.so
;noload => app_controlplayback.so
;noload => app_db.so
;noload => app_dial.so
;noload => app_dictate.so
;noload => app_directed_pickup.so
;noload => app_directory.so
;noload => app_disa.so
;noload => app_dumpchan.so
;noload => app_echo.so
;noload => app_exec.so
;noload => app_externalivr.so
;noload => app_festival.so
;noload => app_followme.so
;noload => app_forkcdr.so
;noload => app_getcpeid.so
;noload => app_ices.so
;noload => app_image.so
;noload => app_ivrdemo.so
;noload => app_jack.so
;noload => app_macro.so
;noload => app_milliwatt.so
;noload => app_minivm.so
;noload => app_mixmonitor.so
;noload => app_morsecode.so
;noload => app_mp3.so
;noload => app_nbscat.so
;noload => app_originate.so
;noload => app_page.so
;noload => app_playback.so
;noload => app_playtones.so
;noload => app_privacy.so
;noload => app_queue.so
;noload => app_readexten.so
;noload => app_read.so
;noload => app_record.so
;noload => app_saycounted.so
;noload => app_sayunixtime.so
;noload => app_senddtmf.so
;noload => app_sendtext.so
;noload => app_skel.so
;noload => app_sms.so
;noload => app_softhangup.so
;noload => app_speech_utils.so
;noload => app_stack.so
;noload => app_stasis.so
;noload => app_statsd.so
;noload => app_stream_echo.so
;noload => app_system.so
;noload => app_talkdetect.so
;noload => app_test.so
;noload => app_transfer.so
;noload => app_url.so
;noload => app_userevent.so
;noload => app_verbose.so
noload => app_voicemail.so
;noload => app_waitforring.so
;noload => app_waitforsilence.so
;noload => app_waituntil.so
;noload => app_while.so
;noload => app_zapateller.so
;
; BRIDGES
;
;noload => bridge_builtin_features.so
;noload => bridge_builtin_interval_features.so
;noload => bridge_holding.so
;noload => bridge_native_rtp.so
;noload => bridge_simple.so
;noload => bridge_softmix.so
;
; CDR
;
;noload => cdr_adaptive_odbc.so
noload => cdr_csv.so
noload => cdr_custom.so
;noload => cdr_manager.so
noload => cdr_pgsql.so
noload => cdr_radius.so
noload => cdr_sqlite3_custom.so
noload => cdr_syslog.so
noload => cdr_tds.so
;
; CEL
;
noload => cel_custom.so
noload => cel_manager.so
noload => cel_odbc.so
noload => cel_pgsql.so
noload => cel_radius.so
noload => cel_sqlite3_custom.so
noload => cel_tds.so
;
; CHANNELS
;
noload => chan_alsa.so
;noload => chan_bridge_media.so
;noload => chan_console.so
noload => chan_iax2.so
noload => chan_mgcp.so
noload => chan_mobile.so
noload => chan_motif.so
noload => chan_ooh323.so
noload => chan_oss.so
noload => chan_phone.so
;noload => chan_pjsip.so
;noload => chan_rtp.so
noload => chan_sip.so
noload => chan_skinny.so
noload => chan_unistim.so
noload => chan_vpb.so
;
; CODECS
;
;noload => codec_adpcm.so
;noload => codec_alaw.so
;noload => codec_a_mu.so
;noload => codec_codec2.so
;noload => codec_g722.so
;noload => codec_g726.s
noload => codec_g729a.so
;noload => codec_gsm.so
;noload => codec_ilbc.so
;noload => codec_lpc10.so
;noload => codec_opus.so
;noload => codec_resample.so
;noload => codec_silk.so
;noload => codec_siren14.so
;noload => codec_siren7.so
;noload => codec_speex.so
;noload => codec_ulaw.so
;
; FORMATS
;
;noload => format_g719.so
;noload => format_g723.so
;noload => format_g726.so
noload => format_g729.so
;noload => format_gsm.so
;noload => format_h263.so
;noload => format_h264.so
;noload => format_ilbc.so
;noload => format_mp3.so
;noload => format_ogg_opus.so
;noload => format_ogg_speex.so
;noload => format_ogg_vorbis.so
;noload => format_pcm.so
;noload => format_siren14.so
;noload => format_siren7.so
;noload => format_sln.so
;noload => format_vox.so
;noload => format_wav_gsm.so
;noload => format_wav.so
;
; FUNCTIONS
;
;noload => func_aes.so
;noload => func_base64.so
;noload => func_blacklist.so
;noload => func_callcompletion.so
;noload => func_callerid.so
;noload => func_cdr.so
;noload => func_channel.so
;noload => func_config.so
;noload => func_curl.so
;noload => func_cut.so
;noload => func_db.so
;noload => func_devstate.so
;noload => func_dialgroup.so
;noload => func_dialplan.so
;noload => func_enum.so
;noload => func_env.so
;noload => func_extstate.so
;noload => func_frame_trace.so
;noload => func_global.so
;noload => func_groupcount.so
;noload => func_hangupcause.so
;noload => func_holdintercept.so
;noload => func_iconv.so
;noload => func_jitterbuffer.so
;noload => func_lock.so
;noload => func_logic.so
;noload => func_math.so
;noload => func_md5.so
;noload => func_module.so
;noload => func_odbc.so
;noload => func_periodic_hook.so
;noload => func_pitchshift.so
;noload => func_pjsip_aor.so
;noload => func_pjsip_contact.so
;noload => func_pjsip_endpoint.so
;noload => func_presencestate.so
;noload => func_rand.so
;noload => func_realtime.so
;noload => func_sha1.so
;noload => func_shell.so
;noload => func_sorcery.so
;noload => func_speex.so
;noload => func_sprintf.so
;noload => func_srv.so
;noload => func_strings.so
;noload => func_sysinfo.so
;noload => func_talkdetect.so
;noload => func_timeout.so
;noload => func_uri.so
;noload => func_version.so
;noload => func_vmcount.so
;noload => func_volume.so
;
; PBX MODULES
;
noload => pbx_ael.so
;noload => pbx_config.so
noload => pbx_dundi.so
;noload => pbx_loopback.so
noload => pbx_lua.so
;noload => pbx_realtime.so
;noload => pbx_spool.so
; 
; RESOURCES
;
;noload => res_adsi.so
noload => res_ael_share.so
noload => res_agi.so
noload => res_ari_applications.so
noload => res_ari_asterisk.so
noload => res_ari_bridges.so
noload => res_ari_channels.so
noload => res_ari_device_states.so
noload => res_ari_endpoints.so
noload => res_ari_events.so
noload => res_ari_mailboxes.so
noload => res_ari_model.so
noload => res_ari_playbacks.so
noload => res_ari_recordings.so
noload => res_ari.so
noload => res_ari_sounds.so
noload => res_calendar_caldav.so
noload => res_calendar_ews.so
noload => res_calendar_exchange.so
noload => res_calendar_icalendar.so
noload => res_calendar.so
;noload => res_chan_stats.so
;noload => res_clialiases.so
;noload => res_clioriginate.so
noload => res_config_curl.so
noload => res_config_ldap.so
noload => res_config_pgsql.so
noload => res_config_sqlite3.so
;noload => res_convert.so
noload => res_corosync.so
;noload => res_crypto.so
;noload => res_curl.so
;noload => res_endpoint_stats.so
noload => res_fax.so
noload => res_fax_spandsp.so
;noload => res_format_attr_celt.so
noload => res_format_attr_g729.so
;noload => res_format_attr_h263.so
;noload => res_format_attr_h264.so
;noload => res_format_attr_ilbc.so
;noload => res_format_attr_opus.so
;noload => res_format_attr_silk.so
;noload => res_format_attr_siren14.so
;noload => res_format_attr_siren7.so
;noload => res_format_attr_vp8.so
noload => res_hep_pjsip.so
noload => res_hep_rtcp.so
noload => res_hep.so
;noload => res_http_media_cache.so
;noload => res_http_post.so
;noload => res_http_websocket.so
;noload => res_limit.so
;noload => res_manager_devicestate.so
;noload => res_manager_presencestate.so
;noload => res_monitor.so
;noload => res_musiconhold.so
;noload => res_mutestream.so
;noload => res_mwi_external_ami.so
;noload => res_odbc.so
;noload => res_odbc_transaction.so
;noload => res_parking.so
noload => res_phoneprov.so
;noload => res_pjproject.so
;noload => res_pjsip_acl.so
;noload => res_pjsip_authenticator_digest.so
;noload => res_pjsip_caller_id.so
;noload => res_pjsip_config_wizard.so
;noload => res_pjsip_dialog_info_body_generator.so
;noload => res_pjsip_diversion.so
;noload => res_pjsip_dlg_options.so
;noload => res_pjsip_dtmf_info.so
;noload => res_pjsip_empty_info.so
;noload => res_pjsip_endpoint_identifier_anonymous.so
;noload => res_pjsip_endpoint_identifier_ip.so
;noload => res_pjsip_endpoint_identifier_user.so
;noload => res_pjsip_exten_state.so
;noload => res_pjsip_header_funcs.so
;noload => res_pjsip_history.so
;noload => res_pjsip_logger.so
;noload => res_pjsip_messaging.so
;noload => res_pjsip_mwi_body_generator.so
;noload => res_pjsip_mwi.so
;noload => res_pjsip_nat.so
;noload => res_pjsip_notify.so
;noload => res_pjsip_one_touch_record_info.so
;noload => res_pjsip_outbound_authenticator_digest.so
;noload => res_pjsip_outbound_publish.so
;noload => res_pjsip_outbound_registration.so
;noload => res_pjsip_path.so
;noload => res_pjsip_phoneprov_provider.so
;noload => res_pjsip_pidf_body_generator.so
;noload => res_pjsip_pidf_digium_body_supplement.so
;noload => res_pjsip_pidf_eyebeam_body_supplement.so
;noload => res_pjsip_publish_asterisk.so
;noload => res_pjsip_pubsub.so
;noload => res_pjsip_refer.so
;noload => res_pjsip_registrar.so
;noload => res_pjsip_rfc3326.so
;noload => res_pjsip_sdp_rtp.so
;noload => res_pjsip_send_to_voicemail.so
;noload => res_pjsip_session.so
;noload => res_pjsip_sips_contact.so
;noload => res_pjsip.so
;noload => res_pjsip_t38.so
;noload => res_pjsip_transport_websocket.so
;noload => res_pjsip_xpidf_body_generator.so
noload => res_pktccops.so
;noload => res_realtime.so
;noload => res_resolver_unbound.so
;noload => res_rtp_asterisk.so
;noload => res_rtp_multicast.so
;noload => res_security_log.so
;noload => res_smdi.so
noload => res_snmp.so
;noload => res_sorcery_astdb.so
;noload => res_sorcery_config.so
;noload => res_sorcery_memory_cache.so
;noload => res_sorcery_memory.so
;noload => res_sorcery_realtime.so
;noload => res_speech.so
;noload => res_srtp.so
;noload => res_stasis_answer.so
;noload => res_stasis_device_state.so
;noload => res_stasis_mailbox.so
;noload => res_stasis_playback.so
;noload => res_stasis_recording.so
;noload => res_stasis_snoop.so
;noload => res_stasis.so
;noload => res_statsd.so
;noload => res_stun_monitor.so
;noload => res_timing_pthread.so
;noload => res_timing_timerfd.so
noload => res_xmpp.so
