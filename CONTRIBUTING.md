# How to contribute to greek-spammers

## How to ask for removal

If you want to be removed from the list open a new issue and provide evidence
that the emails were sent to people who were willingly subscribed/engaged to
your lists.

## How to submit a Pull Request (PR)

If you want to submit a PR, please add as many anonymized headers as possible.
Each PR should only add/remove a single entry to/from the list.

### Headers that should be contained in the PR (if they exist)

1. **From/Return-Path**
1. **Subject**
1. **Date**
1. **Received**
1. **Bounces-To**

### Headers you should anonymize before submitting:
1. **To/X-Original-To/Delivered-To/X-ListMember** 
1. Email address contained in the final **Received**

You can anonymize headers using one of the following ways, choose the one appropriate:
```
* postmaster@domain.tld -> postmaster@*.tld
* username@domain.tld   -> u*@domain.tld
* username@domain.tld   -> u*@*.tld
```

### Headers you may modify before submitting:
1. **Message-ID/X-MessageID**

A spammer may possibly track the *To* address by looking at their logs and the
*Message-ID*, to avoid being detected you may modify that header to whatever
you want.

## Usage of wildcards

Please don't use wildcards unless there are other existing entries from the
same domain in the list or the username part looks random-enough and you have
received multiple emails from the same spammer using different usernames.
