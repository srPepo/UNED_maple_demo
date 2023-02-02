# UNED Abierta Bulk Course Email Template

To add to: `/admin/bulk_email/courseemailtemplate/`.

Add two templates, each one with Name:

* Empty
* Plantilla

Enable bulk emails at: `/admin/bulk_email/bulkemailflag/` with `Enable` checked and `Require course email auth` not checked; or by modifying MySQL database:

```
mysql -u root
use edxapp;
insert into bulk_email_bulkemailflag (change_date, enabled, require_course_email_auth, changed_by_id) values (now(), 1, 0, 5);
```
