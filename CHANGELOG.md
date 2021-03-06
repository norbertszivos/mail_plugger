# Change log


## 1.1.1 (2021-01-21)

### Changes

* Change FakePlugger::DeliveryMethod to returns with the extracted delivery data instead of the message object.
* Update code documentations.
* Add missing FakePlugger description in the README.md.


## 1.1.0 (2021-01-18)

### New features

* Add FakePlugger to mock MailPlugger.

### Changes

* Fix typos in the documentations.
* Add more metadata to gempspec file.


## 1.0.1 (2021-01-15)

### Changes

* Tidy up the gemspec file and change which files contains in the gem. Now the gem is much smaller.
* Add a new mail plugger image which has a different canvas and use it in the README.md.


## 1.0.0 (2021-01-14)

### Changes

* Update gems.
* Remove `webmock` gem to clean up unused things.
* Update documentations.


## 1.0.0.rc1 (2021-01-13)

### Changes

* Change description and fix changelog_uri in gemspec file.
* Add/Change documentations.
* Update gems.
* Change `MailPlugger.plug_in` and `MailPlugger::MailHelper.delivery_options` methods to accept strings and symbols.
* Change `MailPlugger::MailHelper.delivery_data` method that we can retrieve message object as well.
* Check hash keys in `MailPlugger::MailHelper.delivery_system` method, so now if we are add wrong `delivey_system` then we are getting a meaningful error message.
* Change `MailPlugger::MailHelper.extract_attachments` method. If an attachment is inline then the hash contains the `filename` and `cid` as well.
* Add/Change tests.
* Change `MailPlugger::MailHelper.delivery_option` that returns with indifferent hash


## 1.0.0.beta1 (2021-01-02)

* Implement MailPlugger methods and functionality. See [README.md](https://github.com/norbertszivos/mail_plugger/blob/main/README.md)
