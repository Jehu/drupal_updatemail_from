updatemail_from.module
======================

A simple module to use a specific sender email address instead of sites default.  
It also ensures, your mail address is added to the recipient list when update mails are sent.

### Install
* Download module to sites/all/modules
* Enable module "Update Mail From"
* Add variables to settings.php

### Configuration
Admin form will be added soon to avoid editing settings.php.  
Until then these two variables are needed in settings.php to get the module work.   


	/**
	 * Update Mail From module:
	 *
	 * 'updatemail_from_sender' = override the global site email address as sender,
	 * this shold be your key account who decides if an update should take place.
	 * So you can answer the update mail and ask for permission before you make
	 * chargeable updates.
	 *
	 * 'updatemail_from_recipient' = adds an additional recipient for the update
	 * information email. Use this to ensure, you get informed about updates
	 */
	$conf['updatemail_from_sender'] = 'sender@domain.tdl';
	$conf['updatemail_from_recipient'] = 'recipient@other-domain.tdl';