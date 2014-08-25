# Quick API Summary (version 0.1)

## Required

* `/.well-known/smimp.txt`
  * Informs SMIMP clients where to find the SMIMP server for a domain.
* `/version`
  * Gets the SMIMP version from the server (e.g. `0.1` -- denoted `$v` below)
* `/$v/get_user/{address}/{type}`
  * See https://github.com/smimp/smimp_spec/blob/master/smimp_specification.md#get-user-information-required
* `/$v/create_session/{user-address}`
  * https://github.com/smimp/smimp_spec/blob/master/smimp_specification.md#session-management
* `/$v/destroy_session`
* `/$v/get_message_key`
  * https://github.com/smimp/smimp_spec/blob/master/smimp_specification.md#get-message-key-required
* `/$v/send_message/{address}`
  * https://github.com/smimp/smimp_spec/blob/master/smimp_specification.md#send-message-required
* `/$v/folder/{message-type}/{folder-name}`
  * https://github.com/smimp/smimp_spec/blob/master/smimp_specification.md#list-messages-required
* `/$v/message/{message-id}/{update_read}`
  * https://github.com/smimp/smimp_spec/blob/master/smimp_specification.md#get-message-required
* `/$v/message_read/{message_id}`
* `/$v/initialize_account`


## Optional

* `/$v/user_avatar/{address}`
  * https://github.com/smimp/smimp_spec/blob/master/smimp_specification.md#get-user-avatar-optional
* `/$v/get_pow_params/{address}/{message_type}`
  * https://github.com/smimp/smimp_spec/blob/master/smimp_specification.md#get-proof-of-work-parameters-optional
* `/$v/folders/{message-type}`
  * https://github.com/smimp/smimp_spec/blob/master/smimp_specification.md#list-folders-optional
* `/$v/folder/{message-type}/{folder-name}`
  * https://github.com/smimp/smimp_spec/blob/master/smimp_specification.md#rename-folder-optional
* `/$v/message_move/{message-id}`
  * https://github.com/smimp/smimp_spec/blob/master/smimp_specification.md#move-message-optional
* 
