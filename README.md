# Splunk Addon for InQuest

## Table of Contents

### OVERVIEW

- About the Splunk Addon for InQuest
- Release notes
- Support and resources

### INSTALLATION AND CONFIGURATION

- Installation steps
- Configure the Splunk Addon for InQuest

### USER GUIDE

- Features

-----

### OVERVIEW

#### About the Splunk Addon for InQuest

| Author | InQuest Labs |
| --- | --- |
| App Version | 1.0.0 |
| Vendor Products | InQuest 3.80+ |
| Has index-time operations | false |
| Create an index | false |
| Implements summarization | false |

The Splunk Addon for InQuest allows a Splunk® Enterprise administrator t
search and build visualizations and alerts for InQuest device logs.

#### Release notes

##### About this release

Version 1.0.0 of the Splunk Addon for InQuest is compatible with:

| Splunk Enterprise versions | Verified with 6.5 and 6.6 |
| --- | --- |
| CIM | Verified with 4.9.0 |
| Platforms | Platform independent |
| Vendor Products | InQuest 3.80+ |

##### Support and resources

**Support**

Contact support@inquest.net for email support during weekday business hours
(US, East Coast).

## INSTALLATION AND CONFIGURATION

### Software requirements

The Splunk Addon for InQuest has no special software or hardware requirements,
outside of a base Splunk server install.

#### Splunk Enterprise system requirements

Because this add-on runs on Splunk Enterprise, all of the 
[Splunk Enterprise system requirements](http://docs.splunk.com/Documentation/Splunk/latest/Installation/Systemrequirements)
apply.

#### Download

Download the Splunk Addon for InQuest at https://splunkbase.splunk.com/apps/.

#### Installation steps

To install and configure this app on your supported platform, follow these
steps:

1. Install Splunk Addon for InQuest via the Splunk UI.
2. Follow the configuration steps below as applicable for your install.
3. Restart the Splunk server.

#### Configure the Splunk Addon for InQuest

The Splunk Addon for InQuest assumes your InQuest logs are being sent with
sourcetype="syslog". If this is not the case, copy the `props.conf` file
from `$SPLUNK_HOME/etc/apps/TA-inquest/default/props.conf` to 
`$SPLUNK_HOME/etc/apps/TA-inquest/local/props.conf`, and change the section
header from `[syslog]` to whatever sourcetype you wish to use.

## USER GUIDE

### Features

This app provides log field extraction and aliases for the following log types:

- InQuest audit logs
- InQuest engine logs
- InQuest CEF-format logs

All fields include CIM-compliant aliases or extractions as appropriate.
