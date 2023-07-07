# Comparing `tmp/fossbill-0.8.1-py3-none-any.whl.zip` & `tmp/fossbill-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,71 +1,55 @@
-Zip file size: 75018 bytes, number of entries: 69
--rw-r--r--  2.0 unx     1504 b- defN 23-Jul-05 12:26 fossbill/__init__.py
--rw-r--r--  2.0 unx     3177 b- defN 23-Jul-05 12:26 fossbill/alembic.ini
--rw-r--r--  2.0 unx    11111 b- defN 23-Jul-05 12:26 fossbill/auth.py
--rw-r--r--  2.0 unx    28284 b- defN 23-Jul-05 12:26 fossbill/bill.py
--rw-r--r--  2.0 unx     5102 b- defN 23-Jul-05 12:26 fossbill/client.py
--rw-r--r--  2.0 unx     9311 b- defN 23-Jul-05 12:26 fossbill/database.py
--rw-r--r--  2.0 unx      344 b- defN 23-Jul-05 12:26 fossbill/landing.py
--rw-r--r--  2.0 unx     9272 b- defN 23-Jul-05 12:26 fossbill/payment.py
--rw-r--r--  2.0 unx     6679 b- defN 23-Jul-05 12:26 fossbill/product.py
--rw-r--r--  2.0 unx     7098 b- defN 23-Jul-05 12:26 fossbill/user.py
--rw-r--r--  2.0 unx     1836 b- defN 23-Jul-05 12:26 fossbill/alembic/env.py
--rw-r--r--  2.0 unx      510 b- defN 23-Jul-05 12:26 fossbill/alembic/script.py.mako
--rw-r--r--  2.0 unx      611 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/0321467f0761_add_locale_to_user_pref.py
--rw-r--r--  2.0 unx     1323 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/16d25ef8b85d_user_password_reset_token.py
--rw-r--r--  2.0 unx      575 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/277fecce5d8a_drop_bill_amount.py
--rw-r--r--  2.0 unx      697 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/3398d67a1567_add_stripe_customer.py
--rw-r--r--  2.0 unx     1922 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/50c653e9e43d_add_quote_number.py
--rw-r--r--  2.0 unx      850 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/5252d44f6650_unify_currency.py
--rw-r--r--  2.0 unx     1537 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/56f0467e2b79_fixup_nullables.py
--rw-r--r--  2.0 unx      775 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/62c6a992f261_user_password_reset_token_expiration_.py
--rw-r--r--  2.0 unx      658 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/750c2b11b496_add_due_at.py
--rw-r--r--  2.0 unx      912 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/7f2749ea8845_longer_email_address.py
--rw-r--r--  2.0 unx     1257 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/bc99a00f1844_add_payments.py
--rw-r--r--  2.0 unx      697 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/c765c3dc1d91_add_created_at.py
--rw-r--r--  2.0 unx      735 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/dc2ff78bd82b_add_reply_to_and_cc.py
--rw-r--r--  2.0 unx      696 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/deffdb4ce76e_add_user_admin_boolean.py
--rw-r--r--  2.0 unx     6119 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/e88981c927d4_init.py
--rw-r--r--  2.0 unx      697 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/f1ea99885270_add_paid_boolean_on_bills.py
--rw-r--r--  2.0 unx     1163 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/f85e2b7d582a_add_quote_mentions_and_add_them_to_bills.py
--rw-r--r--  2.0 unx      842 b- defN 23-Jul-05 12:26 fossbill/alembic/versions/fda694e67f67_store_payment_payload_required_data.py
--rw-r--r--  2.0 unx      450 b- defN 23-Jul-05 12:26 fossbill/locale/en_US/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx    15871 b- defN 23-Jul-05 12:26 fossbill/locale/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--  2.0 unx      259 b- defN 23-Jul-05 12:26 fossbill/static/bill.css
--rw-r--r--  2.0 unx     2147 b- defN 23-Jul-05 12:26 fossbill/static/style.css
--rw-r--r--  2.0 unx     1331 b- defN 23-Jul-05 12:26 fossbill/templates/base.html
--rw-r--r--  2.0 unx     1588 b- defN 23-Jul-05 12:26 fossbill/templates/macros.html
--rw-r--r--  2.0 unx      395 b- defN 23-Jul-05 12:26 fossbill/templates/auth/ask_reset_password.html
--rw-r--r--  2.0 unx      670 b- defN 23-Jul-05 12:26 fossbill/templates/auth/login.html
--rw-r--r--  2.0 unx      538 b- defN 23-Jul-05 12:26 fossbill/templates/auth/register.html
--rw-r--r--  2.0 unx      152 b- defN 23-Jul-05 12:26 fossbill/templates/auth/reset_password_email.plain
--rw-r--r--  2.0 unx      518 b- defN 23-Jul-05 12:26 fossbill/templates/auth/use_reset_password.html
--rw-r--r--  2.0 unx      107 b- defN 23-Jul-05 12:26 fossbill/templates/bill/bill_email.plain
--rw-r--r--  2.0 unx      598 b- defN 23-Jul-05 12:26 fossbill/templates/bill/create.html
--rw-r--r--  2.0 unx     1247 b- defN 23-Jul-05 12:26 fossbill/templates/bill/generated_bill.html
--rw-r--r--  2.0 unx     2384 b- defN 23-Jul-05 12:26 fossbill/templates/bill/generated_quote.html
--rw-r--r--  2.0 unx     5373 b- defN 23-Jul-05 12:26 fossbill/templates/bill/index.html
--rw-r--r--  2.0 unx      108 b- defN 23-Jul-05 12:26 fossbill/templates/bill/quote_email.plain
--rw-r--r--  2.0 unx      732 b- defN 23-Jul-05 12:26 fossbill/templates/bill/send_bill_email.html
--rw-r--r--  2.0 unx      733 b- defN 23-Jul-05 12:26 fossbill/templates/bill/send_quote_email.html
--rw-r--r--  2.0 unx     7949 b- defN 23-Jul-05 12:26 fossbill/templates/bill/update.html
--rw-r--r--  2.0 unx     1039 b- defN 23-Jul-05 12:26 fossbill/templates/bill/update_bill.html
--rw-r--r--  2.0 unx     3428 b- defN 23-Jul-05 12:26 fossbill/templates/bill/update_quote.html
--rw-r--r--  2.0 unx     1193 b- defN 23-Jul-05 12:26 fossbill/templates/client/create.html
--rw-r--r--  2.0 unx     1981 b- defN 23-Jul-05 12:26 fossbill/templates/client/index.html
--rw-r--r--  2.0 unx     1553 b- defN 23-Jul-05 12:26 fossbill/templates/client/update.html
--rw-r--r--  2.0 unx      815 b- defN 23-Jul-05 12:26 fossbill/templates/landing/dashboard.html
--rw-r--r--  2.0 unx     1194 b- defN 23-Jul-05 12:26 fossbill/templates/landing/welcome.html
--rw-r--r--  2.0 unx     3308 b- defN 23-Jul-05 12:26 fossbill/templates/payment/home.html
--rw-r--r--  2.0 unx     1381 b- defN 23-Jul-05 12:26 fossbill/templates/payment/invoice.html
--rw-r--r--  2.0 unx     1155 b- defN 23-Jul-05 12:26 fossbill/templates/product/create.html
--rw-r--r--  2.0 unx     2566 b- defN 23-Jul-05 12:26 fossbill/templates/product/index.html
--rw-r--r--  2.0 unx     1492 b- defN 23-Jul-05 12:26 fossbill/templates/product/update.html
--rw-r--r--  2.0 unx       91 b- defN 23-Jul-05 12:26 fossbill/templates/user/test_email.plain
--rw-r--r--  2.0 unx     5939 b- defN 23-Jul-05 12:26 fossbill/templates/user/update.html
--rw-r--r--  2.0 unx    34523 b- defN 23-Jul-05 12:27 fossbill-0.8.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      232 b- defN 23-Jul-05 12:27 fossbill-0.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-05 12:27 fossbill-0.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-05 12:27 fossbill-0.8.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6678 b- defN 23-Jul-05 12:27 fossbill-0.8.1.dist-info/RECORD
-69 files, 218113 bytes uncompressed, 64092 bytes compressed:  70.6%
+Zip file size: 65659 bytes, number of entries: 53
+-rw-r--r--  2.0 unx     1504 b- defN 23-Jul-07 07:57 fossbill/__init__.py
+-rw-r--r--  2.0 unx     3177 b- defN 23-Jul-07 07:57 fossbill/alembic.ini
+-rw-r--r--  2.0 unx    11111 b- defN 23-Jul-07 07:57 fossbill/auth.py
+-rw-r--r--  2.0 unx    28284 b- defN 23-Jul-07 07:57 fossbill/bill.py
+-rw-r--r--  2.0 unx     5102 b- defN 23-Jul-07 07:57 fossbill/client.py
+-rw-r--r--  2.0 unx     9311 b- defN 23-Jul-07 07:57 fossbill/database.py
+-rw-r--r--  2.0 unx      344 b- defN 23-Jul-07 07:57 fossbill/landing.py
+-rw-r--r--  2.0 unx     9272 b- defN 23-Jul-07 07:57 fossbill/payment.py
+-rw-r--r--  2.0 unx     6679 b- defN 23-Jul-07 07:57 fossbill/product.py
+-rw-r--r--  2.0 unx    12061 b- defN 23-Jul-07 07:57 fossbill/user.py
+-rw-r--r--  2.0 unx     1836 b- defN 23-Jul-07 07:57 fossbill/alembic/env.py
+-rw-r--r--  2.0 unx      510 b- defN 23-Jul-07 07:57 fossbill/alembic/script.py.mako
+-rw-r--r--  2.0 unx     7758 b- defN 23-Jul-07 07:57 fossbill/alembic/versions/fda694e67f67_init.py
+-rw-r--r--  2.0 unx      450 b- defN 23-Jul-07 07:57 fossbill/locale/en_US/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx    15918 b- defN 23-Jul-07 07:57 fossbill/locale/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--  2.0 unx      259 b- defN 23-Jul-07 07:57 fossbill/static/bill.css
+-rw-r--r--  2.0 unx     2164 b- defN 23-Jul-07 07:57 fossbill/static/style.css
+-rw-r--r--  2.0 unx     1331 b- defN 23-Jul-07 07:57 fossbill/templates/base.html
+-rw-r--r--  2.0 unx     1588 b- defN 23-Jul-07 07:57 fossbill/templates/macros.html
+-rw-r--r--  2.0 unx      395 b- defN 23-Jul-07 07:57 fossbill/templates/auth/ask_reset_password.html
+-rw-r--r--  2.0 unx      670 b- defN 23-Jul-07 07:57 fossbill/templates/auth/login.html
+-rw-r--r--  2.0 unx      538 b- defN 23-Jul-07 07:57 fossbill/templates/auth/register.html
+-rw-r--r--  2.0 unx      152 b- defN 23-Jul-07 07:57 fossbill/templates/auth/reset_password_email.plain
+-rw-r--r--  2.0 unx      518 b- defN 23-Jul-07 07:57 fossbill/templates/auth/use_reset_password.html
+-rw-r--r--  2.0 unx      107 b- defN 23-Jul-07 07:57 fossbill/templates/bill/bill_email.plain
+-rw-r--r--  2.0 unx      598 b- defN 23-Jul-07 07:57 fossbill/templates/bill/create.html
+-rw-r--r--  2.0 unx     1247 b- defN 23-Jul-07 07:57 fossbill/templates/bill/generated_bill.html
+-rw-r--r--  2.0 unx     2384 b- defN 23-Jul-07 07:57 fossbill/templates/bill/generated_quote.html
+-rw-r--r--  2.0 unx     5373 b- defN 23-Jul-07 07:57 fossbill/templates/bill/index.html
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-07 07:57 fossbill/templates/bill/quote_email.plain
+-rw-r--r--  2.0 unx      732 b- defN 23-Jul-07 07:57 fossbill/templates/bill/send_bill_email.html
+-rw-r--r--  2.0 unx      733 b- defN 23-Jul-07 07:57 fossbill/templates/bill/send_quote_email.html
+-rw-r--r--  2.0 unx     7949 b- defN 23-Jul-07 07:57 fossbill/templates/bill/update.html
+-rw-r--r--  2.0 unx     1039 b- defN 23-Jul-07 07:57 fossbill/templates/bill/update_bill.html
+-rw-r--r--  2.0 unx     3428 b- defN 23-Jul-07 07:57 fossbill/templates/bill/update_quote.html
+-rw-r--r--  2.0 unx     1193 b- defN 23-Jul-07 07:57 fossbill/templates/client/create.html
+-rw-r--r--  2.0 unx     1981 b- defN 23-Jul-07 07:57 fossbill/templates/client/index.html
+-rw-r--r--  2.0 unx     1553 b- defN 23-Jul-07 07:57 fossbill/templates/client/update.html
+-rw-r--r--  2.0 unx      836 b- defN 23-Jul-07 07:57 fossbill/templates/landing/dashboard.html
+-rw-r--r--  2.0 unx     1194 b- defN 23-Jul-07 07:57 fossbill/templates/landing/welcome.html
+-rw-r--r--  2.0 unx     3308 b- defN 23-Jul-07 07:57 fossbill/templates/payment/home.html
+-rw-r--r--  2.0 unx     1381 b- defN 23-Jul-07 07:57 fossbill/templates/payment/invoice.html
+-rw-r--r--  2.0 unx     1155 b- defN 23-Jul-07 07:57 fossbill/templates/product/create.html
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jul-07 07:57 fossbill/templates/product/index.html
+-rw-r--r--  2.0 unx     1492 b- defN 23-Jul-07 07:57 fossbill/templates/product/update.html
+-rw-r--r--  2.0 unx      630 b- defN 23-Jul-07 07:57 fossbill/templates/user/import_export_user.html
+-rw-r--r--  2.0 unx       91 b- defN 23-Jul-07 07:57 fossbill/templates/user/test_email.plain
+-rw-r--r--  2.0 unx     6041 b- defN 23-Jul-07 07:57 fossbill/templates/user/update.html
+-rw-r--r--  2.0 unx    34523 b- defN 23-Jul-07 07:59 fossbill-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      232 b- defN 23-Jul-07 07:59 fossbill-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 07:59 fossbill-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-07 07:59 fossbill-0.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4749 b- defN 23-Jul-07 07:59 fossbill-0.9.0.dist-info/RECORD
+53 files, 207656 bytes uncompressed, 58007 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -30,66 +30,15 @@
 
 Filename: fossbill/alembic/env.py
 Comment: 
 
 Filename: fossbill/alembic/script.py.mako
 Comment: 
 
-Filename: fossbill/alembic/versions/0321467f0761_add_locale_to_user_pref.py
-Comment: 
-
-Filename: fossbill/alembic/versions/16d25ef8b85d_user_password_reset_token.py
-Comment: 
-
-Filename: fossbill/alembic/versions/277fecce5d8a_drop_bill_amount.py
-Comment: 
-
-Filename: fossbill/alembic/versions/3398d67a1567_add_stripe_customer.py
-Comment: 
-
-Filename: fossbill/alembic/versions/50c653e9e43d_add_quote_number.py
-Comment: 
-
-Filename: fossbill/alembic/versions/5252d44f6650_unify_currency.py
-Comment: 
-
-Filename: fossbill/alembic/versions/56f0467e2b79_fixup_nullables.py
-Comment: 
-
-Filename: fossbill/alembic/versions/62c6a992f261_user_password_reset_token_expiration_.py
-Comment: 
-
-Filename: fossbill/alembic/versions/750c2b11b496_add_due_at.py
-Comment: 
-
-Filename: fossbill/alembic/versions/7f2749ea8845_longer_email_address.py
-Comment: 
-
-Filename: fossbill/alembic/versions/bc99a00f1844_add_payments.py
-Comment: 
-
-Filename: fossbill/alembic/versions/c765c3dc1d91_add_created_at.py
-Comment: 
-
-Filename: fossbill/alembic/versions/dc2ff78bd82b_add_reply_to_and_cc.py
-Comment: 
-
-Filename: fossbill/alembic/versions/deffdb4ce76e_add_user_admin_boolean.py
-Comment: 
-
-Filename: fossbill/alembic/versions/e88981c927d4_init.py
-Comment: 
-
-Filename: fossbill/alembic/versions/f1ea99885270_add_paid_boolean_on_bills.py
-Comment: 
-
-Filename: fossbill/alembic/versions/f85e2b7d582a_add_quote_mentions_and_add_them_to_bills.py
-Comment: 
-
-Filename: fossbill/alembic/versions/fda694e67f67_store_payment_payload_required_data.py
+Filename: fossbill/alembic/versions/fda694e67f67_init.py
 Comment: 
 
 Filename: fossbill/locale/en_US/LC_MESSAGES/messages.mo
 Comment: 
 
 Filename: fossbill/locale/fr_FR/LC_MESSAGES/messages.mo
 Comment: 
@@ -180,29 +129,32 @@
 
 Filename: fossbill/templates/product/index.html
 Comment: 
 
 Filename: fossbill/templates/product/update.html
 Comment: 
 
+Filename: fossbill/templates/user/import_export_user.html
+Comment: 
+
 Filename: fossbill/templates/user/test_email.plain
 Comment: 
 
 Filename: fossbill/templates/user/update.html
 Comment: 
 
-Filename: fossbill-0.8.1.dist-info/LICENSE
+Filename: fossbill-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: fossbill-0.8.1.dist-info/METADATA
+Filename: fossbill-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: fossbill-0.8.1.dist-info/WHEEL
+Filename: fossbill-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: fossbill-0.8.1.dist-info/top_level.txt
+Filename: fossbill-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fossbill-0.8.1.dist-info/RECORD
+Filename: fossbill-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fossbill/user.py

```diff
@@ -1,20 +1,23 @@
 from flask import (
     Blueprint, flash, g, current_app, redirect, render_template, request, url_for,
-    session
+    session, send_file
 )
 from werkzeug.exceptions import abort
 from fossbill.auth import login_required, user_pref_smtp_enough
 from fossbill.database import get_db
 from fossbill.auth import setup_locale
 from fossbill.auth import load_logged_in_user
 from sqlalchemy import insert, select
 from sqlalchemy.exc import SQLAlchemyError
 import smtplib
 from email.message import EmailMessage
+import tarfile
+import io
+import csv
 
 bp = Blueprint('user', __name__, url_prefix='/me')
 
 def get_user_smtp_server(user_pref):
     if user_pref.smtp_security == "TLS":
         server = smtplib.SMTP_SSL(
             host=user_pref.smtp_host,
@@ -219,7 +222,159 @@
             conn.commit()
             flash(_("All bills has been deleted."))
     except SQLAlchemyError as e:
         current_app.logger.error(str(e))
         flash(_("Something went wrong."))
 
     return redirect(url_for("user.update"))
+
+@bp.route('/import_export_user')
+@login_required
+def import_export_user():
+    return render_template('user/import_export_user.html')
+
+@bp.route('/import_user', methods=['POST'])
+@login_required
+def import_user():
+    error = None
+    if 'file' not in request.files or request.files['file'].filename == '':
+        error = _('File is required.')
+
+    if error is None:
+        file = tarfile.open(fileobj=request.files['file'].stream)
+
+        try:
+            import_user_tar_file(file)
+        except KeyError as e:
+            error = _("The file format seems incorrect.")
+        except SQLAlchemyError as e:
+            current_app.logger.error(str(e))
+            error = _("Something went wrong.")
+        else:
+            flash(_("User data imported."))
+            return redirect(url_for("landing.home"))
+
+    flash(error)
+    return redirect(url_for("user.import_export_user"))
+
+def import_user_tar_file(file):
+    engine, metadata = get_db()
+    with engine.connect() as conn:
+        for table_name in ['bill_row', 'bill', 'client', 'product']:
+            table = metadata.tables[table_name]
+            stmt = table.delete().where(
+                table.c.user_id == g.user.id,
+            )
+            conn.execute(stmt)
+
+        clientfile = io.TextIOWrapper(file.extractfile('client.csv'))
+        clientreader = csv.reader(clientfile)
+        clientids = {}
+        for row in clientreader:
+            stmt = insert(metadata.tables['client']).values(
+                address=row[1],
+                email=row[2],
+                label=row[3],
+                user_id=g.user.id,
+            )
+            result = conn.execute(stmt)
+            clientids[row[0]] = result.inserted_primary_key[0]
+
+        productfile = io.TextIOWrapper(file.extractfile('product.csv'))
+        productreader = csv.reader(productfile)
+        for row in productreader:
+            stmt = insert(metadata.tables['product']).values(
+                label=row[0],
+                price=row[1],
+                tax_rate=row[2],
+                user_id=g.user.id,
+            )
+            conn.execute(stmt)
+
+        billfile = io.TextIOWrapper(file.extractfile('bill.csv'))
+        billreader = csv.reader(billfile)
+        billids = {}
+        for row in billreader:
+            stmt = insert(metadata.tables['bill']).values(
+                client_id=clientids[row[1]] or None,
+                comment=row[2],
+                date=row[3],
+                bill_number=row[4] or None,
+                quote_number=row[5] or None,
+                recipient=row[6],
+                source=row[7],
+                bill_mentions=row[7],
+                quote_mentions=row[9],
+                paid=row[10] == 'False',
+                user_id=g.user.id,
+            )
+            result = conn.execute(stmt)
+            billids[row[0]] = result.inserted_primary_key[0]
+
+        billrowfile = io.TextIOWrapper(file.extractfile('bill_row.csv'))
+        billrowreader = csv.reader(billrowfile)
+        for row in billrowreader:
+            stmt = insert(metadata.tables['bill_row']).values(
+                bill_id=billids[row[0]],
+                label=row[1],
+                price=row[2],
+                quantity=row[3],
+                tax_rate=row[4],
+                user_id=g.user.id,
+            )
+            conn.execute(stmt)
+
+        conn.commit()
+
+@bp.route('/export_user')
+@login_required
+def export_user():
+    tarfilebuf = io.BytesIO()
+    file = tarfile.open(fileobj=tarfilebuf, mode='w:bz2')
+
+    add_tarfile_from_table(file, 'client', ['id', 'address', 'email', 'label'])
+    add_tarfile_from_table(file, 'product', ['label', 'price', 'tax_rate'])
+    add_tarfile_from_table(file, 'bill', [
+        'id',
+        'client_id',
+        'comment',
+        'date',
+        'bill_number',
+        'quote_number',
+        'recipient',
+        'source',
+        'bill_mentions',
+        'quote_mentions',
+        'paid'
+    ])
+    add_tarfile_from_table(file, 'bill_row', [
+        'bill_id',
+        'label',
+        'price',
+        'quantity',
+        'tax_rate',
+    ])
+
+    file.close()
+
+    tarfilebuf.seek(0)
+
+    return send_file(tarfilebuf, download_name="fossbill_export.tar.bz2")
+
+def add_tarfile_from_table(file, table, columns):
+    engine, metadata = get_db()
+    with engine.connect() as conn:
+        filebuf = io.BytesIO()
+        textbuf = io.TextIOWrapper(filebuf)
+        writer = csv.writer(textbuf)
+        stmt = select(metadata.tables[table]).where(
+            metadata.tables[table].c.user_id == g.user.id,
+        )
+        result = conn.execute(stmt)
+        rows = result.fetchall()
+        for row in rows:
+            writer.writerow([getattr(row, column) for column in columns])
+        textbuf.flush()
+        filebuf.seek(0)
+        info = tarfile.TarInfo('{}.csv'.format(table))
+        info.size=filebuf.getbuffer().nbytes
+        file.addfile(tarinfo=info, fileobj=filebuf)
```

## fossbill/locale/en_US/LC_MESSAGES/messages.mo

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: fossbill 0.3.0*

```diff
@@ -3,15 +3,15 @@
 00000020: 2c00 0000 9401 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2066 6f73 7362 696c 6c20 302e 332e 300a   fossbill 0.3.0.
 00000050: 5265 706f 7274 2d4d 7367 6964 2d42 7567  Report-Msgid-Bug
 00000060: 732d 546f 3a20 454d 4149 4c40 4144 4452  s-To: EMAIL@ADDR
 00000070: 4553 530a 504f 542d 4372 6561 7469 6f6e  ESS.POT-Creation
 00000080: 2d44 6174 653a 2032 3032 332d 3037 2d30  -Date: 2023-07-0
-00000090: 3520 3130 3a30 302b 3032 3030 0a50 4f2d  5 10:00+0200.PO-
+00000090: 3520 3131 3a33 342b 3032 3030 0a50 4f2d  5 11:34+0200.PO-
 000000a0: 5265 7669 7369 6f6e 2d44 6174 653a 2032  Revision-Date: 2
 000000b0: 3032 332d 3034 2d32 3420 3132 3a31 342b  023-04-24 12:14+
 000000c0: 3032 3030 0a4c 6173 742d 5472 616e 736c  0200.Last-Transl
 000000d0: 6174 6f72 3a20 4655 4c4c 204e 414d 4520  ator: FULL NAME 
 000000e0: 3c45 4d41 494c 4041 4444 5245 5353 3e0a  <EMAIL@ADDRESS>.
 000000f0: 4c61 6e67 7561 6765 3a20 656e 5f55 530a  Language: en_US.
 00000100: 4c61 6e67 7561 6765 2d54 6561 6d3a 2065  Language-Team: e
```

## fossbill/locale/fr_FR/LC_MESSAGES/messages.mo

### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: fossbill 0.3.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-07-05 10:00+0200\n"
+"POT-Creation-Date: 2023-07-05 11:34+0200\n"
 "PO-Revision-Date: 2023-04-24 13:12+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fr_FR\n"
 "Language-Team: fr_FR <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -130,19 +130,19 @@
 msgid "Bill updated."
 msgstr "Facture modifiée."
 
 msgid "Bills"
 msgstr "Factures"
 
 msgid ""
-"Bills will be Quotes untill you \"finish\" them. A unique bill number will "
-"then be applied on them."
+"Bills will be Drafts untill you generate a Quote or directly a Bill from "
+"them. Unique numbers will be applied on them."
 msgstr ""
-"Les factures seront des brouillons jusqu'à ce que vous les \"valider\". Un "
-"numéro unique leur sera ensuite appliqués."
+"Les factures seront des brouillons jusqu'à ce que vous génériez le devis ou "
+"directement la facture. Des numéro uniques leur seront appliqué"
 
 msgid "Body"
 msgstr "Corp"
 
 msgid "Body is required."
 msgstr "Corp requis."
```

## fossbill/static/style.css

```diff
@@ -1,11 +1,11 @@
 html { font-family: sans-serif; background-color: #303030; color: #eaeaea; }
 a { color: #377ba8; }
 input.danger { color: #cc2f2e; }
-input, select, textarea, #card-element { background-color: #eaeaea; }
+input:not([type=file]), select, textarea, #card-element { background-color: #eaeaea; }
 body { max-width: 960px; margin: 1rem auto 3rem auto; }
 nav { display: flex; align-items: flex-end; justify-content: space-between; }
 ul { padding: 0; }
 nav > * { margin: 0; }
 nav h1 { font-size: 2rem; }
 nav ul { display: flex; list-style: none; }
 nav ul > *:not(:first-child) { display: block; margin-left: 1rem; }
```

## fossbill/templates/landing/dashboard.html

```diff
@@ -3,10 +3,10 @@
 {% block header %}
   <h1>{% block title %}{% trans %}Dashboard{% endtrans %}{% endblock %}</h1>
 {% endblock %}
 
 {% block content %}
   <p>{% trans %}Thanks a lot for registering, and welcome aboard! Fossbill is a really simple tool. Here some guidelines:{% endtrans %}</p>
   <p>{% trans %}You should start by editing your user preference. Then add some products you use frequently. You can also prepare your client list. Registering products and clients isnt necessary but it make generating bills faster.{% endtrans %}</p>
-  <p>{% trans %}Bills will be Quotes untill you "finish" them. A unique bill number will then be applied on them.{% endtrans %}</p>
+  <p>{% trans %}Bills will be Drafts untill you generate a Quote or directly a Bill from them. Unique numbers will be applied on them.{% endtrans %}</p>
   <p>{% trans %}You can preview and also send them to any email address you want, as quote or bill.{% endtrans %}</p>
 {% endblock %}
```

## fossbill/templates/user/update.html

```diff
@@ -96,9 +96,10 @@
       </form>
       <form action="{{ url_for('user.delete') }}" method="post">
         <input class="danger" type="submit" value="{% trans %}Delete user{% endtrans %}" onclick="return confirm('{% trans %}You are about to delete all data associated to this account.\nAre you sure?{% endtrans %}');">
       </form>
       <form action="{{ url_for('user.delete_bills') }}" method="post">
         <input class="danger" type="submit" value="{% trans %}Delete bills{% endtrans %}" onclick="return confirm('{% trans %}You are about to delete all of your bills.\nAre you sure?{% endtrans %}');">
       </form>
+      <a href="{{ url_for('user.import_export_user') }}">{% trans %}Import / Export{% endtrans %}</a>
   </div>
 {% endblock %}
```

## Comparing `fossbill/alembic/versions/e88981c927d4_init.py` & `fossbill/alembic/versions/fda694e67f67_init.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,132 +1,158 @@
-"""Init
+"""init
 
-Revision ID: e88981c927d4
+Revision ID: fda694e67f67
 Revises: 
-Create Date: 2023-02-08 14:22:03.272820
+Create Date: 2023-07-05 11:39:05.497527
 
 """
 from alembic import op
 import sqlalchemy as sa
-from fossbill.database import get_db
-from sqlalchemy import inspect
 
 
 # revision identifiers, used by Alembic.
-revision = 'e88981c927d4'
+revision = 'fda694e67f67'
 down_revision = None
 branch_labels = None
 depends_on = None
 
 
 def upgrade() -> None:
-    engine, metadata = get_db()
-    insp = inspect(engine)
-    tables = insp.get_table_names()
-
-    if 'user' not in tables:
-        op.create_table('user',
-            sa.Column('id', sa.Integer(), nullable=False),
-            sa.Column('password', sa.String(length=120), nullable=False),
-            sa.Column('username', sa.String(length=50), nullable=False),
-            sa.PrimaryKeyConstraint('id'),
-            sa.UniqueConstraint('username')
-        )
-
-    if 'client' not in tables:
-        op.create_table('client',
-            sa.Column('address', sa.String(length=500), nullable=True),
-            sa.Column('currency', sa.String(length=10), nullable=True),
-            sa.Column('email', sa.String(length=70), nullable=True),
-            sa.Column('id', sa.Integer(), nullable=False),
-            sa.Column('label', sa.String(length=40), nullable=False),
-            sa.Column('user_id', sa.Integer(), nullable=False),
-            sa.ForeignKeyConstraint(['user_id'], ['user.id'], ),
-            sa.PrimaryKeyConstraint('id')
-        )
-        op.create_index(op.f('ix_client_user_id'), 'client', ['user_id'], unique=False)
-
-    if 'product' not in tables:
-        op.create_table('product',
-            sa.Column('id', sa.Integer(), nullable=False),
-            sa.Column('label', sa.String(length=120), nullable=False),
-            sa.Column('price', sa.Integer(), nullable=False),
-            sa.Column('tax_rate', sa.Integer(), nullable=False),
-            sa.Column('user_id', sa.Integer(), nullable=False),
-            sa.ForeignKeyConstraint(['user_id'], ['user.id'], ),
-            sa.PrimaryKeyConstraint('id')
-        )
-        op.create_index(op.f('ix_product_user_id'), 'product', ['user_id'], unique=False)
-
-    if 'user_pref' not in tables:
-        op.create_table('user_pref',
-            sa.Column('currency', sa.String(length=10), nullable=True),
-            sa.Column('email', sa.String(length=70), nullable=True),
-            sa.Column('id', sa.Integer(), nullable=False),
-            sa.Column('mentions', sa.String(length=500), nullable=True),
-            sa.Column('smtp_host', sa.String(length=30), nullable=True),
-            sa.Column('smtp_password', sa.String(length=30), nullable=True),
-            sa.Column('smtp_port', sa.Integer(), nullable=True),
-            sa.Column('smtp_security', sa.String(length=10), nullable=True),
-            sa.Column('smtp_username', sa.String(length=30), nullable=True),
-            sa.Column('source', sa.String(length=500), nullable=True),
-            sa.Column('user_id', sa.Integer(), nullable=False),
-            sa.ForeignKeyConstraint(['user_id'], ['user.id'], ),
-            sa.PrimaryKeyConstraint('id')
-        )
-        op.create_index(op.f('ix_user_pref_user_id'), 'user_pref', ['user_id'], unique=False)
-
-    if 'bill' not in tables:
-        op.create_table('bill',
-            sa.Column('amount', sa.Integer(), nullable=False),
-            sa.Column('client_id', sa.Integer(), nullable=True),
-            sa.Column('comment', sa.String(length=500), nullable=True),
-            sa.Column('currency', sa.String(length=10), nullable=True),
-            sa.Column('date', sa.Date(), nullable=False),
-            sa.Column('draft', sa.Boolean(), nullable=False),
-            sa.Column('id', sa.Integer(), nullable=False),
-            sa.Column('number', sa.Integer(), nullable=True),
-            sa.Column('recipient', sa.String(length=500), nullable=False),
-            sa.Column('source', sa.String(length=500), nullable=False),
-            sa.Column('user_id', sa.Integer(), nullable=False),
-            sa.CheckConstraint('draft is TRUE or number is not NULL'),
-            sa.ForeignKeyConstraint(['client_id'], ['client.id'], ),
-            sa.ForeignKeyConstraint(['user_id'], ['user.id'], ),
-            sa.PrimaryKeyConstraint('id'),
-            sa.UniqueConstraint('user_id', 'number')
-        )
-        op.create_index(op.f('ix_bill_client_id'), 'bill', ['client_id'], unique=False)
-        op.create_index(op.f('ix_bill_number'), 'bill', ['number'], unique=False)
-        op.create_index(op.f('ix_bill_user_id'), 'bill', ['user_id'], unique=False)
-
-    if 'bill_row' not in tables:
-        op.create_table('bill_row',
-            sa.Column('bill_id', sa.Integer(), nullable=False),
-            sa.Column('id', sa.Integer(), nullable=False),
-            sa.Column('label', sa.String(length=120), nullable=False),
-            sa.Column('price', sa.Integer(), nullable=False),
-            sa.Column('quantity', sa.Integer(), nullable=False),
-            sa.Column('tax_rate', sa.Integer(), nullable=False),
-            sa.Column('user_id', sa.Integer(), nullable=False),
-            sa.ForeignKeyConstraint(['bill_id'], ['bill.id'], ),
-            sa.ForeignKeyConstraint(['user_id'], ['user.id'], ),
-            sa.PrimaryKeyConstraint('id')
-        )
-        op.create_index(op.f('ix_bill_row_bill_id'), 'bill_row', ['bill_id'], unique=False)
-        op.create_index(op.f('ix_bill_row_user_id'), 'bill_row', ['user_id'], unique=False)
+    # ### commands auto generated by Alembic - please adjust! ###
+    op.create_table('user',
+    sa.Column('id', sa.Integer(), nullable=False),
+    sa.Column('username', sa.String(length=50), nullable=False),
+    sa.Column('password', sa.String(length=120), nullable=False),
+    sa.Column('stripe_customer', sa.String(length=256), nullable=True),
+    sa.Column('admin', sa.Boolean(), nullable=False),
+    sa.Column('due_at', sa.Date(), nullable=True),
+    sa.Column('created_at', sa.Date(), server_default=sa.text('CURRENT_DATE'), nullable=False),
+    sa.PrimaryKeyConstraint('id'),
+    sa.UniqueConstraint('username')
+    )
+    op.create_table('client',
+    sa.Column('id', sa.Integer(), nullable=False),
+    sa.Column('address', sa.String(length=500), nullable=False),
+    sa.Column('email', sa.String(length=70), nullable=False),
+    sa.Column('label', sa.String(length=40), nullable=False),
+    sa.Column('user_id', sa.Integer(), nullable=False),
+    sa.ForeignKeyConstraint(['user_id'], ['user.id'], ),
+    sa.PrimaryKeyConstraint('id')
+    )
+    op.create_index(op.f('ix_client_user_id'), 'client', ['user_id'], unique=False)
+    op.create_table('payment',
+    sa.Column('id', sa.Integer(), nullable=False),
+    sa.Column('user_id', sa.Integer(), nullable=False),
+    sa.Column('date', sa.Date(), nullable=False),
+    sa.Column('valid_for_service_thru', sa.Date(), nullable=False),
+    sa.Column('amount', sa.Integer(), nullable=False),
+    sa.Column('currency', sa.String(length=10), nullable=True),
+    sa.Column('payload', sa.JSON(), nullable=True),
+    sa.Column('card_brand', sa.String(length=20), nullable=True),
+    sa.Column('card_last4', sa.String(length=4), nullable=True),
+    sa.ForeignKeyConstraint(['user_id'], ['user.id'], ),
+    sa.PrimaryKeyConstraint('id')
+    )
+    op.create_index(op.f('ix_payment_user_id'), 'payment', ['user_id'], unique=False)
+    op.create_table('product',
+    sa.Column('id', sa.Integer(), nullable=False),
+    sa.Column('label', sa.String(length=120), nullable=False),
+    sa.Column('price', sa.Integer(), nullable=False),
+    sa.Column('tax_rate', sa.Integer(), nullable=False),
+    sa.Column('user_id', sa.Integer(), nullable=False),
+    sa.ForeignKeyConstraint(['user_id'], ['user.id'], ),
+    sa.PrimaryKeyConstraint('id')
+    )
+    op.create_index(op.f('ix_product_user_id'), 'product', ['user_id'], unique=False)
+    op.create_table('user_password_reset_token',
+    sa.Column('id', sa.Integer(), nullable=False),
+    sa.Column('user_id', sa.Integer(), nullable=False),
+    sa.Column('token', sa.String(length=128), nullable=False),
+    sa.Column('expire_at', sa.DateTime(), server_default=sa.text('now()'), nullable=False),
+    sa.ForeignKeyConstraint(['user_id'], ['user.id'], ),
+    sa.PrimaryKeyConstraint('id'),
+    sa.UniqueConstraint('token')
+    )
+    op.create_index(op.f('ix_user_password_reset_token_user_id'), 'user_password_reset_token', ['user_id'], unique=False)
+    op.create_table('user_pref',
+    sa.Column('bill_mentions', sa.String(length=500), nullable=True),
+    sa.Column('currency', sa.String(length=10), nullable=True),
+    sa.Column('email', sa.String(length=254), nullable=True),
+    sa.Column('id', sa.Integer(), nullable=False),
+    sa.Column('locale', sa.String(length=10), nullable=False),
+    sa.Column('quote_mentions', sa.String(length=500), nullable=True),
+    sa.Column('smtp_host', sa.String(length=30), nullable=True),
+    sa.Column('smtp_password', sa.String(length=30), nullable=True),
+    sa.Column('smtp_port', sa.Integer(), nullable=True),
+    sa.Column('smtp_security', sa.String(length=10), nullable=True),
+    sa.Column('smtp_username', sa.String(length=30), nullable=True),
+    sa.Column('smtp_reply_to', sa.String(length=254), nullable=True),
+    sa.Column('smtp_cc', sa.String(length=508), nullable=True),
+    sa.Column('source', sa.String(length=500), nullable=True),
+    sa.Column('user_id', sa.Integer(), nullable=False),
+    sa.ForeignKeyConstraint(['user_id'], ['user.id'], ),
+    sa.PrimaryKeyConstraint('id'),
+    sa.UniqueConstraint('email')
+    )
+    op.create_index(op.f('ix_user_pref_user_id'), 'user_pref', ['user_id'], unique=False)
+    op.create_table('bill',
+    sa.Column('id', sa.Integer(), nullable=False),
+    sa.Column('client_id', sa.Integer(), nullable=True),
+    sa.Column('comment', sa.String(length=500), nullable=True),
+    sa.Column('date', sa.Date(), nullable=False),
+    sa.Column('bill_number', sa.Integer(), nullable=True),
+    sa.Column('quote_number', sa.Integer(), nullable=True),
+    sa.Column('recipient', sa.String(length=500), nullable=True),
+    sa.Column('source', sa.String(length=500), nullable=True),
+    sa.Column('user_id', sa.Integer(), nullable=False),
+    sa.Column('bill_mentions', sa.String(length=500), nullable=True),
+    sa.Column('quote_mentions', sa.String(length=500), nullable=True),
+    sa.Column('paid', sa.Boolean(), server_default='FALSE', nullable=False),
+    sa.ForeignKeyConstraint(['client_id'], ['client.id'], ),
+    sa.ForeignKeyConstraint(['user_id'], ['user.id'], ),
+    sa.PrimaryKeyConstraint('id'),
+    sa.UniqueConstraint('user_id', 'bill_number'),
+    sa.UniqueConstraint('user_id', 'quote_number')
+    )
+    op.create_index(op.f('ix_bill_bill_number'), 'bill', ['bill_number'], unique=False)
+    op.create_index(op.f('ix_bill_client_id'), 'bill', ['client_id'], unique=False)
+    op.create_index(op.f('ix_bill_quote_number'), 'bill', ['quote_number'], unique=False)
+    op.create_index(op.f('ix_bill_user_id'), 'bill', ['user_id'], unique=False)
+    op.create_table('bill_row',
+    sa.Column('bill_id', sa.Integer(), nullable=False),
+    sa.Column('id', sa.Integer(), nullable=False),
+    sa.Column('label', sa.String(length=120), nullable=False),
+    sa.Column('price', sa.Integer(), nullable=False),
+    sa.Column('quantity', sa.Integer(), nullable=False),
+    sa.Column('tax_rate', sa.Integer(), nullable=False),
+    sa.Column('user_id', sa.Integer(), nullable=False),
+    sa.ForeignKeyConstraint(['bill_id'], ['bill.id'], ),
+    sa.ForeignKeyConstraint(['user_id'], ['user.id'], ),
+    sa.PrimaryKeyConstraint('id')
+    )
+    op.create_index(op.f('ix_bill_row_bill_id'), 'bill_row', ['bill_id'], unique=False)
+    op.create_index(op.f('ix_bill_row_user_id'), 'bill_row', ['user_id'], unique=False)
+    # ### end Alembic commands ###
 
 
 def downgrade() -> None:
+    # ### commands auto generated by Alembic - please adjust! ###
     op.drop_index(op.f('ix_bill_row_user_id'), table_name='bill_row')
     op.drop_index(op.f('ix_bill_row_bill_id'), table_name='bill_row')
     op.drop_table('bill_row')
     op.drop_index(op.f('ix_bill_user_id'), table_name='bill')
-    op.drop_index(op.f('ix_bill_number'), table_name='bill')
+    op.drop_index(op.f('ix_bill_quote_number'), table_name='bill')
     op.drop_index(op.f('ix_bill_client_id'), table_name='bill')
+    op.drop_index(op.f('ix_bill_bill_number'), table_name='bill')
     op.drop_table('bill')
     op.drop_index(op.f('ix_user_pref_user_id'), table_name='user_pref')
     op.drop_table('user_pref')
+    op.drop_index(op.f('ix_user_password_reset_token_user_id'), table_name='user_password_reset_token')
+    op.drop_table('user_password_reset_token')
     op.drop_index(op.f('ix_product_user_id'), table_name='product')
     op.drop_table('product')
+    op.drop_index(op.f('ix_payment_user_id'), table_name='payment')
+    op.drop_table('payment')
     op.drop_index(op.f('ix_client_user_id'), table_name='client')
     op.drop_table('client')
     op.drop_table('user')
+    # ### end Alembic commands ###
```

## Comparing `fossbill-0.8.1.dist-info/LICENSE` & `fossbill-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

