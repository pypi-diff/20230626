# Comparing `tmp/aws_adfs-2.7.0.tar.gz` & `tmp/aws_adfs-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_adfs-2.7.0.tar", max compression
+gzip compressed data, was "aws_adfs-2.8.0.tar", max compression
```

## Comparing `aws_adfs-2.7.0.tar` & `aws_adfs-2.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1070 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/LICENSE
--rw-r--r--   0        0        0    14886 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/README.md
--rw-r--r--   0        0        0      159 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/__init__.py
--rw-r--r--   0        0        0     3541 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/_azure_cloud_mfa_authenticator.py
--rw-r--r--   0        0        0     1848 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/_azure_mfa_authenticator.py
--rw-r--r--   0        0        0    20501 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/_duo_authenticator.py
--rw-r--r--   0        0        0    21283 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/_duo_universal_prompt_authenticator.py
--rw-r--r--   0        0        0     2124 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/_rsa_authenticator.py
--rw-r--r--   0        0        0     2450 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/_symantec_vip_access.py
--rw-r--r--   0        0        0     1518 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/account_aliases_fetcher.py
--rw-r--r--   0        0        0     7373 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/authenticator.py
--rw-r--r--   0        0        0     1327 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/commands.py
--rw-r--r--   0        0        0      217 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/consts.py
--rw-r--r--   0        0        0      856 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/helpers.py
--rw-r--r--   0        0        0     4161 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/html_roles_fetcher.py
--rw-r--r--   0        0        0      778 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/list_profiles.py
--rw-r--r--   0        0        0    24810 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/login.py
--rw-r--r--   0        0        0    10918 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/prepare.py
--rw-r--r--   0        0        0     1243 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/reset.py
--rw-r--r--   0        0        0     2457 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/role_chooser.py
--rw-r--r--   0        0        0     3729 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/roles_assertion_extractor.py
--rw-r--r--   0        0        0     1509 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/pyproject.toml
--rw-r--r--   0        0        0    16445 1970-01-01 00:00:00.000000 aws_adfs-2.7.0/setup.py
--rw-r--r--   0        0        0    16428 1970-01-01 00:00:00.000000 aws_adfs-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/LICENSE
+-rw-r--r--   0        0        0    14887 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/README.md
+-rw-r--r--   0        0        0      159 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/__init__.py
+-rw-r--r--   0        0        0     3985 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/_azure_cloud_mfa_authenticator.py
+-rw-r--r--   0        0        0     1848 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/_azure_mfa_authenticator.py
+-rw-r--r--   0        0        0    20501 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/_duo_authenticator.py
+-rw-r--r--   0        0        0    21389 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/_duo_universal_prompt_authenticator.py
+-rw-r--r--   0        0        0     2124 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/_rsa_authenticator.py
+-rw-r--r--   0        0        0     2450 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/_symantec_vip_access.py
+-rw-r--r--   0        0        0     1518 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/account_aliases_fetcher.py
+-rw-r--r--   0        0        0     7373 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/authenticator.py
+-rw-r--r--   0        0        0     1327 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/commands.py
+-rw-r--r--   0        0        0      217 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/consts.py
+-rw-r--r--   0        0        0      856 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/helpers.py
+-rw-r--r--   0        0        0     4161 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/html_roles_fetcher.py
+-rw-r--r--   0        0        0      778 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/list_profiles.py
+-rw-r--r--   0        0        0    24810 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/login.py
+-rw-r--r--   0        0        0    10918 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/prepare.py
+-rw-r--r--   0        0        0     1243 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/reset.py
+-rw-r--r--   0        0        0     2457 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/role_chooser.py
+-rw-r--r--   0        0        0     3729 2023-06-26 14:00:36.936893 aws_adfs-2.8.0/aws_adfs/roles_assertion_extractor.py
+-rw-r--r--   0        0        0     1509 2023-06-26 14:00:36.940893 aws_adfs-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0    16446 1970-01-01 00:00:00.000000 aws_adfs-2.8.0/setup.py
+-rw-r--r--   0        0        0    16429 1970-01-01 00:00:00.000000 aws_adfs-2.8.0/PKG-INFO
```

### Comparing `aws_adfs-2.7.0/LICENSE` & `aws_adfs-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.7.0/README.md` & `aws_adfs-2.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -381,13 +381,13 @@
 poetry run pytest
 ```
 
 * release:
 
 ```
 export CHANGELOG_GITHUB_TOKEN=$(gopass show -o pins/Github/github-changelog-generator)
-./script/release.sh patch # or minor, major, prepatch, preminor, premajor, prerelease, or a valid semver string
+./scripts/release.sh patch # or minor, major, prepatch, preminor, premajor, prerelease, or a valid semver string
 ```
 
 ## Changelog
 
 See the [CHANGELOG.md](CHANGELOG.md) file, which is generated using [github-changelog-generator](https://github.com/github-changelog-generator/github-changelog-generator).
```

### Comparing `aws_adfs-2.7.0/aws_adfs/_azure_cloud_mfa_authenticator.py` & `aws_adfs-2.8.0/aws_adfs/_azure_cloud_mfa_authenticator.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,18 +30,24 @@
         aad_verification_code
     )
 
 def _retrieve_roles_page(html_response, session, ssl_verification_enabled, aad_verification_code):
     seconds_to_wait = 5
     max_attempts = 12
     counter = 1
+    has_number_matching = False
 
     while True:
         time.sleep(seconds_to_wait)
 
+        number_to_match = _number_matching(html_response)
+        if number_to_match and not has_number_matching:
+            has_number_matching = True
+            click.echo(number_to_match, err=True)
+
         aad_verification_code_text = _aad_verification_code_text(html_response)
         if aad_verification_code_text is not None:
             seconds_to_wait = 0
             if aad_verification_code is None:
                 aad_verification_code = click.prompt(aad_verification_code_text)
 
         response = session.post(
@@ -99,7 +105,12 @@
     element = html_response.find(mfa_instructions_query)
     return element.text if element is not None else ''
 
 def _aad_verification_code_text(html_response):
     aad_verification_code_query = './/input[@id="verificationCodeInput"]'
     element = html_response.find(aad_verification_code_query)
     return None if element is None else element.get('placeholder')
+
+def _number_matching(html_response):
+    number_matching_query = './/p[@id="validEntropyNumber"]'
+    element = html_response.find(number_matching_query)
+    return None if element is None else element.text
```

### Comparing `aws_adfs-2.7.0/aws_adfs/_azure_mfa_authenticator.py` & `aws_adfs-2.8.0/aws_adfs/_azure_mfa_authenticator.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.7.0/aws_adfs/_duo_authenticator.py` & `aws_adfs-2.8.0/aws_adfs/_duo_authenticator.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.7.0/aws_adfs/_duo_universal_prompt_authenticator.py` & `aws_adfs-2.8.0/aws_adfs/_duo_universal_prompt_authenticator.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 try:
     from fido2.pcsc import CtapPcscDevice
 except ImportError:
     CtapPcscDevice = None
 
 import logging
 import json
+import platform
 import re
 
 from threading import Event, Thread
 
 from .consts import (
     DUO_UNIVERSAL_PROMPT_FACTOR_DUO_PUSH,
     DUO_UNIVERSAL_PROMPT_FACTOR_PHONE_CALL,
@@ -34,15 +35,17 @@
     from urlparse import urlparse, parse_qs
     import Queue as queue
 
 from . import roles_assertion_extractor
 
 _headers = {
     "Accept-Language": "en",
-    "User-Agent": "Mozilla/5.0 (Windows NT 6.1; WOW64; Trident/7.0; rv:11.0) like Gecko",
+    "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) like Gecko"
+    if platform.system() == "Linux"
+    else "Mozilla/5.0 (Windows NT 6.1; WOW64; Trident/7.0; rv:11.0) like Gecko",
     "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
     "Accept": "text/plain, */*; q=0.01",
 }
 
 
 def extract(html_response, ssl_verification_enabled, session, duo_factor, duo_device):
     """
```

### Comparing `aws_adfs-2.7.0/aws_adfs/_rsa_authenticator.py` & `aws_adfs-2.8.0/aws_adfs/_rsa_authenticator.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.7.0/aws_adfs/_symantec_vip_access.py` & `aws_adfs-2.8.0/aws_adfs/_symantec_vip_access.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.7.0/aws_adfs/account_aliases_fetcher.py` & `aws_adfs-2.8.0/aws_adfs/account_aliases_fetcher.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.7.0/aws_adfs/authenticator.py` & `aws_adfs-2.8.0/aws_adfs/authenticator.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.7.0/aws_adfs/commands.py` & `aws_adfs-2.8.0/aws_adfs/commands.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.7.0/aws_adfs/helpers.py` & `aws_adfs-2.8.0/aws_adfs/helpers.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.7.0/aws_adfs/html_roles_fetcher.py` & `aws_adfs-2.8.0/aws_adfs/html_roles_fetcher.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.7.0/aws_adfs/list_profiles.py` & `aws_adfs-2.8.0/aws_adfs/list_profiles.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.7.0/aws_adfs/login.py` & `aws_adfs-2.8.0/aws_adfs/login.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.7.0/aws_adfs/prepare.py` & `aws_adfs-2.8.0/aws_adfs/prepare.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.7.0/aws_adfs/reset.py` & `aws_adfs-2.8.0/aws_adfs/reset.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.7.0/aws_adfs/role_chooser.py` & `aws_adfs-2.8.0/aws_adfs/role_chooser.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.7.0/aws_adfs/roles_assertion_extractor.py` & `aws_adfs-2.8.0/aws_adfs/roles_assertion_extractor.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.7.0/pyproject.toml` & `aws_adfs-2.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool]
 [tool.poetry]
 name = "aws-adfs"
-version = "2.7.0"
+version = "2.8.0"
 description = "AWS CLI authenticator via ADFS - small command-line tool to authenticate via ADFS and assume chosen role"
 keywords = ["aws", "adfs", "console", "tool"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Developers",
```

### Comparing `aws_adfs-2.7.0/setup.py` & `aws_adfs-2.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,17 +21,17 @@
  ':platform_system == "Windows"': ['requests-negotiate-sspi>=0.5,<0.6']}
 
 entry_points = \
 {'console_scripts': ['aws-adfs = aws_adfs.commands:cli']}
 
 setup_kwargs = {
     'name': 'aws-adfs',
-    'version': '2.7.0',
+    'version': '2.8.0',
     'description': 'AWS CLI authenticator via ADFS - small command-line tool to authenticate via ADFS and assume chosen role',
-    'long_description': '# aws-adfs\n[![PyPI version](https://badge.fury.io/py/aws-adfs.svg)](https://badge.fury.io/py/aws-adfs)\n[![Travis build](https://api.travis-ci.org/venth/aws-adfs.svg?branch=master)](https://api.travis-ci.org/venth/aws-adfs.svg?branch=master)\n![Build Status](https://github.com/venth/aws-adfs/workflows/Build/badge.svg?branch=master)\n\nThe project provides command line tool - `aws-adfs` to ease AWS cli authentication against ADFS (multi factor authentication with active directory).\n\n## `aws-adfs` command line tool\n\n* allows you to re-login to STS without entering credentials for an extended period of time, without having to store the user\'s actual credentials. It also lets an organization control the period in which a user can re-login to STS without entering credentials, by altering the ADFS session lifetime.\n\n* supports automation tools like ansible by providing security token in `AWS_SESSION_TOKEN`/`AWS_SECURITY_TOKEN` environment variables.\n\n* supports using Security Support Provider Interface (SSPI) on Windows OS.\n\n### MFA integration\n\naws-adfs integrates with:\n* [duo security](https://duo.com) MFA provider with support for:\n  * Duo mobile application push (verified by code or not) using the `Duo Push` authentication method.\n  * Phone call using the `Phone Call` authentication method.\n  * OTP 6 digit codes generated by Duo Mobile application, and hardware tokens (e.g. RSA or Yubikey) using the `Passcode` authentication method.\n  * FIDO U2F (CTAP1) / FIDO2 (CTAP2) hardware authenticators using the `WebAuthn Security Key` authentication method.\n* [Symantec VIP](https://vip.symantec.com/) MFA provider\n* [RSA SecurID](https://www.rsa.com/) MFA provider\n* [Azure AD MFA](https://learn.microsoft.com/en-us/azure/active-directory/authentication/concept-mfa-howitworks) with support for:\n  * Microsoft Authenticator app\n  * OTP 6 digit codes\n  * SMS codes\n  * Phone call\n\n## Setup Dependencies\n\n- `build-essential` (provides C/C++ compilers)\n- `python3` `>= 3.7 <4.0`\n- `python3-dev`\n- `libkrb5-dev`\n- `libxml2-dev`\n\n## Installation\n\n* user local installation with [pipx](https://github.com/pypa/pipx)\n\n    ```\n    pipx install aws-adfs\n    ```\n\n* user local installation with pip\n\n    ```\n    pip3 install --user aws-adfs\n    ```\n\n    Please note, that you need to add $HOME/.local/bin to your PATH\n\n* system wide installation\n\n    ```\n    sudo pip3 install aws-adfs\n    ```\n\n* virtualenvs\n\n    ```\n    virtualenv aws-adfs\n    source aws-adfs/bin/activate\n    pip install aws-adfs\n    ...\n    ...\n    deactivate\n    ```\n\n* Windows 10\n\n   - Install latest supported Visual C++ downloads from Microsoft for Visual Studio 2015, 2017 and 2019:\n      - https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads\n      - https://aka.ms/vs/16/release/vc_redist.x64.exe\n    - Install Python 3.7 from Microsoft Store:\n      - https://www.microsoft.com/en-us/p/python-37/9nj46sx7x90p\n    - Start PowerShell as Administrator\n    - Go to `C:\\Program Files`:\n        ```\n        C:\n        cd \'C:\\Program Files\\\'\n        ```\n    - Create virtual env:\n      ```\n      python3 -m venv aws-adfs\n      ```\n    - Install `aws-adfs`:\n      ```\n      & \'C:\\Program Files\\aws-adfs\\Scripts\\pip\' install aws-adfs\n      ```\n    - Run it:\n      ```\n      & \'C:\\Program Files\\aws-adfs\\Scripts\\aws-adfs\' login --adfs-host=your-adfs-hostname\n      ```\n\n## Examples of usage\n\n### `aws-adfs`\n* login to your adfs host with disabled ssl verification on aws cli profile: adfs\n\n    ```\n    aws-adfs login --adfs-host=your-adfs-hostname --no-ssl-verification\n    ```\n\n    and verification\n\n    ```\n    aws --profile=adfs s3 ls\n    ```\n\n* login to your adfs host with disabled ssl verification on specified aws cli profile: specified-profile\n\n    ```\n    aws-adfs login --profile=specified-profile --adfs-host=your-adfs-hostname --no-ssl-verification\n    ```\n\n    and verification\n\n    ```\n    aws --profile=specified-profile s3 ls\n    ```\n\n* login to your adfs host and fetch roles for AWS GovCloud (US)\n\n    ```\n    aws-adfs login --adfs-host=your-adfs-hostname --provider-id urn:amazon:webservices:govcloud --region us-gov-west-1\n    ```\n\n    and verification\n\n    ```\n    aws s3 ls\n    ```\n\n* login to your adfs host within ansible playbook\n\n    ```\n    ---\n    - name: "Auth sts aws"\n      command: "aws-adfs login --adfs-host sts.example.com --env --stdout --role-arn arn:aws:iam::000123456789:role/ADMIN"\n      register: sts_result\n      environment:\n        - username: "{{ ansible_user }}@example.com"\n        - password: "{{ ansible_ssh_pass }}"\n\n    - name: "Set sts facts"\n      set_fact:\n        sts: "{{ sts_result.stdout | from_json }}"\n\n    - name: "List s3 Buckets"\n      aws_s3_bucket_facts:\n        aws_access_key: "{{\xa0sts.AccessKeyId }}"\n        aws_secret_key: "{{\xa0sts.SecretAccessKey }}"\n        security_token: "{{\xa0sts.SessionToken }}"\n        region: "us-east-1"\n      register: buckets\n\n    - name: "Print Buckets"\n      debug:\n        var: buckets\n    ```\n\n* login to your adfs host by passing username and password credentials via a file\n\n    ```\n    aws-adfs login --adfs-host=your-adfs-hostname --authfile=/path/and/file/name\n    ```\n\n    Auth file should be in format of\n\n    ```\n    [profile_name]\n    username = your_username\n    password = your_password\n    ```\n\n* .aws/config profile for automatically refreshing credentials\n    ```\n    [profile example-role-ue1]\n    credential_process=aws-adfs login --region=us-east-1 --role-arn=arn:aws:iam::1234567891234:role/example-role --adfs-host=adfs.example.com --stdout\n    ```\n    Warning: see [AWS documentation](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-sourcing-external.html) about security considerations to take when sourcing credentials with an external process.\n\n* help, help, help?\n    <!-- AWS_HELP_START -->\n    ```\n    $ aws-adfs --help\n    Usage: aws-adfs [OPTIONS] COMMAND [ARGS]...\n\n    Options:\n      --version      Show current tool version\n      -v, --verbose  Enables debug information on stdout. By default log level is\n                     set on ERROR\n      --help         Show this message and exit.\n\n    Commands:\n      list   lists available profiles\n      login  Authenticates an user with active directory credentials\n      reset  removes stored profile\n    ```\n    <!-- AWS_HELP_END -->\n\n    <!-- AWS_LIST_HELP_START -->\n    ```\n    $ aws-adfs list --help\n    Usage: aws-adfs list [OPTIONS]\n\n      lists available profiles\n\n    Options:\n      --help  Show this message and exit.\n    ```\n    <!-- AWS_LIST_HELP_END -->\n\n    <!-- AWS_LOGIN_HELP_START -->\n    ```\n    $ aws-adfs login --help\n    Usage: aws-adfs login [OPTIONS]\n\n      Authenticates an user with active directory credentials\n\n    Options:\n      --profile TEXT                  AWS cli profile that will be authenticated.\n                                      After successful authentication just use:\n                                      aws --profile <authenticated profile>\n                                      <service> ...\n      --region TEXT                   The default AWS region that this script will\n                                      connect to for all API calls\n      --ssl-verification / --no-ssl-verification\n                                      SSL certificate verification: Whether or not\n                                      strict certificate verification is done,\n                                      False should only be used for dev/test\n      --adfs-ca-bundle TEXT           Override CA bundle for SSL certificate\n                                      verification for ADFS server only.\n      --adfs-host TEXT                For the first time for a profile it has to\n                                      be provided, next time for the same profile\n                                      it will be loaded from the stored\n                                      configuration\n      --output-format [json|text|table]\n                                      Output format used by aws cli\n      --provider-id TEXT              Provider ID, e.g urn:amazon:webservices\n                                      (optional)\n      --s3-signature-version [s3v4]   s3 signature version: Identifies the version\n                                      of AWS Signature to support for\n                                      authenticated requests. Valid values: s3v4\n      --username-password-command TEXT\n                                      Read username and password from the output\n                                      of a shell command (expected JSON format:\n                                      `{"username": "myusername", "password":\n                                      "mypassword"}`)\n      --env                           Read username, password from environment\n                                      variables (username and password).\n      --stdin                         Read username, password from standard input\n                                      separated by a newline.\n      --authfile TEXT                 Read username, password from a local file\n                                      (optional)\n      --stdout                        Print aws_session_token in json on stdout.\n      --printenv                      Output commands to set AWS_ACCESS_KEY_ID,\n                                      AWS_SECRET_ACCESS_KEY, AWS_SESSION_TOKEN,\n                                      AWS_DEFAULT_REGION environmental variables\n                                      instead of saving them to the aws\n                                      configuration file.\n      --print-console-signin-url      Output a URL that lets users who sign in to\n                                      your organization\'s network securely access\n                                      the AWS Management Console.\n      --console-role-arn TEXT         Role to assume for use in conjunction with\n                                      --print-console-signin-url\n      --console-external-id TEXT      External ID to pass in assume role for use\n                                      in conjunction with --print-console-signin-\n                                      url\n      --role-arn TEXT                 Predefined role arn to selects, e.g. aws-\n                                      adfs login --role-arn arn:aws:iam::123456789\n                                      012:role/YourSpecialRole\n      --session-duration INTEGER      Define the amount of seconds you want to\n                                      establish your STS session, e.g. aws-adfs\n                                      login --session-duration 3600\n      --no-session-cache              Do not use AWS session cache in\n                                      ~/.aws/adfs_cache/ directory.\n      --assertfile TEXT               Use SAML assertion response from a local\n                                      file\n      --sspi / --no-sspi              Whether or not to use Kerberos SSO\n                                      authentication via SSPI (Windows only,\n                                      defaults to True).\n      --duo-factor TEXT               Use a specific Duo factor, overriding the\n                                      default one configured server side. Known\n                                      Duo factors that can be used with aws-adfs\n                                      are "Duo Push", "Passcode", "Phone Call" and\n                                      "WebAuthn Security Key".\n      --duo-device TEXT               Use a specific Duo device, overriding the\n                                      default one configured server side. Depends\n                                      heavily on the Duo factor used. Known Duo\n                                      devices that can be used with aws-adfs are\n                                      "phone1" for "Duo Push" and "Phone Call"\n                                      factors. For "Passcode" and "WebAuthn\n                                      Security Key" factors, it is always "None".\n      --enforce-role-arn              Only allow the role passed in by --role-arn.\n      --aad-verification-code TEXT    Verification code for Azure AD multi-factor\n                                      authentication.\n      --help                          Show this message and exit.\n    ```\n    <!-- AWS_LOGIN_HELP_END -->\n\n    <!-- AWS_RESET_HELP_START -->\n    ```\n    $ aws-adfs reset --help\n    Usage: aws-adfs reset [OPTIONS]\n\n      removes stored profile\n\n    Options:\n      --profile TEXT  AWS cli profile that will be removed\n      --help          Show this message and exit.\n    ```\n    <!-- AWS_RESET_HELP_END -->\n\n## Known issues\n\n* duo-security\n\n    `Error: Cannot begin authentication process. The error response: {"message": "Unknown authentication method.", "stat": "FAIL"}`\n\n    Please setup preferred auth method in duo-security settings (settings\' -> \'My Settings & Devices\').\n\n* USB FIDO2 does not work in Windows Subsystem for Linux (WSL)\n\n    `OSError: [Errno 2] No such file or directory: \'/sys/class/hidraw\'`\n\n    USB devices are not accessible in WSL, please install and run `aws-adfs` on the Windows 10 host and then access the credentials in WSL from the filesystem. Example:\n\n    ```\n    export AWS_CONFIG_FILE=/mnt/c/Users/username/.aws/config\n    export AWS_SHARED_CREDENTIALS_FILE=/mnt/c/Users/username/.aws/credentials\n    ```\n\n*  FIDO2 devices are not detected on Windows 10 build 1903 or newer\n\n    Running `aws-adfs` as Administrator is required since Windows 10 build 1903 to access FIDO2 devices, cf. https://github.com/Yubico/python-fido2/issues/55)\n\n* in cases of trouble with lxml please install\n\n  ```\n  sudo apt-get install python3-dev libxml2-dev libxslt1-dev zlib1g-dev\n  ```\n\n* in cases of trouble with pykerberos please install\n\n  ```\n  sudo apt-get install python3-dev libkrb5-dev\n  ```\n\n* in cases of trouble with OSX Sierra (obsolete OpenSSL), upgrade OpenSSL. Example:\n  ```\n  brew upgrade openssl\n  ```\n  AND add explicit directive to .bash_profile:\n  ```\n  export PATH=$(brew --prefix openssl)/bin:$PATH\n  ```\n\n* only python >= 3.7 to <4.0 are supported:\n  - python 2.6 is not supported\n  - python 2.7 is not supported\n  - python 3.2 is not supported\n  - python 3.3 is not supported\n  - python 3.4 is not supported\n  - python 3.5 is not supported\n  - python 3.6 is not supported\n\n## Development\n\n* update dependencies:\n```\npoetry update\n```\n\n* run unit tests:\n```\npoetry run pytest\n```\n\n* release:\n\n```\nexport CHANGELOG_GITHUB_TOKEN=$(gopass show -o pins/Github/github-changelog-generator)\n./script/release.sh patch # or minor, major, prepatch, preminor, premajor, prerelease, or a valid semver string\n```\n\n## Changelog\n\nSee the [CHANGELOG.md](CHANGELOG.md) file, which is generated using [github-changelog-generator](https://github.com/github-changelog-generator/github-changelog-generator).\n',
+    'long_description': '# aws-adfs\n[![PyPI version](https://badge.fury.io/py/aws-adfs.svg)](https://badge.fury.io/py/aws-adfs)\n[![Travis build](https://api.travis-ci.org/venth/aws-adfs.svg?branch=master)](https://api.travis-ci.org/venth/aws-adfs.svg?branch=master)\n![Build Status](https://github.com/venth/aws-adfs/workflows/Build/badge.svg?branch=master)\n\nThe project provides command line tool - `aws-adfs` to ease AWS cli authentication against ADFS (multi factor authentication with active directory).\n\n## `aws-adfs` command line tool\n\n* allows you to re-login to STS without entering credentials for an extended period of time, without having to store the user\'s actual credentials. It also lets an organization control the period in which a user can re-login to STS without entering credentials, by altering the ADFS session lifetime.\n\n* supports automation tools like ansible by providing security token in `AWS_SESSION_TOKEN`/`AWS_SECURITY_TOKEN` environment variables.\n\n* supports using Security Support Provider Interface (SSPI) on Windows OS.\n\n### MFA integration\n\naws-adfs integrates with:\n* [duo security](https://duo.com) MFA provider with support for:\n  * Duo mobile application push (verified by code or not) using the `Duo Push` authentication method.\n  * Phone call using the `Phone Call` authentication method.\n  * OTP 6 digit codes generated by Duo Mobile application, and hardware tokens (e.g. RSA or Yubikey) using the `Passcode` authentication method.\n  * FIDO U2F (CTAP1) / FIDO2 (CTAP2) hardware authenticators using the `WebAuthn Security Key` authentication method.\n* [Symantec VIP](https://vip.symantec.com/) MFA provider\n* [RSA SecurID](https://www.rsa.com/) MFA provider\n* [Azure AD MFA](https://learn.microsoft.com/en-us/azure/active-directory/authentication/concept-mfa-howitworks) with support for:\n  * Microsoft Authenticator app\n  * OTP 6 digit codes\n  * SMS codes\n  * Phone call\n\n## Setup Dependencies\n\n- `build-essential` (provides C/C++ compilers)\n- `python3` `>= 3.7 <4.0`\n- `python3-dev`\n- `libkrb5-dev`\n- `libxml2-dev`\n\n## Installation\n\n* user local installation with [pipx](https://github.com/pypa/pipx)\n\n    ```\n    pipx install aws-adfs\n    ```\n\n* user local installation with pip\n\n    ```\n    pip3 install --user aws-adfs\n    ```\n\n    Please note, that you need to add $HOME/.local/bin to your PATH\n\n* system wide installation\n\n    ```\n    sudo pip3 install aws-adfs\n    ```\n\n* virtualenvs\n\n    ```\n    virtualenv aws-adfs\n    source aws-adfs/bin/activate\n    pip install aws-adfs\n    ...\n    ...\n    deactivate\n    ```\n\n* Windows 10\n\n   - Install latest supported Visual C++ downloads from Microsoft for Visual Studio 2015, 2017 and 2019:\n      - https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads\n      - https://aka.ms/vs/16/release/vc_redist.x64.exe\n    - Install Python 3.7 from Microsoft Store:\n      - https://www.microsoft.com/en-us/p/python-37/9nj46sx7x90p\n    - Start PowerShell as Administrator\n    - Go to `C:\\Program Files`:\n        ```\n        C:\n        cd \'C:\\Program Files\\\'\n        ```\n    - Create virtual env:\n      ```\n      python3 -m venv aws-adfs\n      ```\n    - Install `aws-adfs`:\n      ```\n      & \'C:\\Program Files\\aws-adfs\\Scripts\\pip\' install aws-adfs\n      ```\n    - Run it:\n      ```\n      & \'C:\\Program Files\\aws-adfs\\Scripts\\aws-adfs\' login --adfs-host=your-adfs-hostname\n      ```\n\n## Examples of usage\n\n### `aws-adfs`\n* login to your adfs host with disabled ssl verification on aws cli profile: adfs\n\n    ```\n    aws-adfs login --adfs-host=your-adfs-hostname --no-ssl-verification\n    ```\n\n    and verification\n\n    ```\n    aws --profile=adfs s3 ls\n    ```\n\n* login to your adfs host with disabled ssl verification on specified aws cli profile: specified-profile\n\n    ```\n    aws-adfs login --profile=specified-profile --adfs-host=your-adfs-hostname --no-ssl-verification\n    ```\n\n    and verification\n\n    ```\n    aws --profile=specified-profile s3 ls\n    ```\n\n* login to your adfs host and fetch roles for AWS GovCloud (US)\n\n    ```\n    aws-adfs login --adfs-host=your-adfs-hostname --provider-id urn:amazon:webservices:govcloud --region us-gov-west-1\n    ```\n\n    and verification\n\n    ```\n    aws s3 ls\n    ```\n\n* login to your adfs host within ansible playbook\n\n    ```\n    ---\n    - name: "Auth sts aws"\n      command: "aws-adfs login --adfs-host sts.example.com --env --stdout --role-arn arn:aws:iam::000123456789:role/ADMIN"\n      register: sts_result\n      environment:\n        - username: "{{ ansible_user }}@example.com"\n        - password: "{{ ansible_ssh_pass }}"\n\n    - name: "Set sts facts"\n      set_fact:\n        sts: "{{ sts_result.stdout | from_json }}"\n\n    - name: "List s3 Buckets"\n      aws_s3_bucket_facts:\n        aws_access_key: "{{\xa0sts.AccessKeyId }}"\n        aws_secret_key: "{{\xa0sts.SecretAccessKey }}"\n        security_token: "{{\xa0sts.SessionToken }}"\n        region: "us-east-1"\n      register: buckets\n\n    - name: "Print Buckets"\n      debug:\n        var: buckets\n    ```\n\n* login to your adfs host by passing username and password credentials via a file\n\n    ```\n    aws-adfs login --adfs-host=your-adfs-hostname --authfile=/path/and/file/name\n    ```\n\n    Auth file should be in format of\n\n    ```\n    [profile_name]\n    username = your_username\n    password = your_password\n    ```\n\n* .aws/config profile for automatically refreshing credentials\n    ```\n    [profile example-role-ue1]\n    credential_process=aws-adfs login --region=us-east-1 --role-arn=arn:aws:iam::1234567891234:role/example-role --adfs-host=adfs.example.com --stdout\n    ```\n    Warning: see [AWS documentation](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-sourcing-external.html) about security considerations to take when sourcing credentials with an external process.\n\n* help, help, help?\n    <!-- AWS_HELP_START -->\n    ```\n    $ aws-adfs --help\n    Usage: aws-adfs [OPTIONS] COMMAND [ARGS]...\n\n    Options:\n      --version      Show current tool version\n      -v, --verbose  Enables debug information on stdout. By default log level is\n                     set on ERROR\n      --help         Show this message and exit.\n\n    Commands:\n      list   lists available profiles\n      login  Authenticates an user with active directory credentials\n      reset  removes stored profile\n    ```\n    <!-- AWS_HELP_END -->\n\n    <!-- AWS_LIST_HELP_START -->\n    ```\n    $ aws-adfs list --help\n    Usage: aws-adfs list [OPTIONS]\n\n      lists available profiles\n\n    Options:\n      --help  Show this message and exit.\n    ```\n    <!-- AWS_LIST_HELP_END -->\n\n    <!-- AWS_LOGIN_HELP_START -->\n    ```\n    $ aws-adfs login --help\n    Usage: aws-adfs login [OPTIONS]\n\n      Authenticates an user with active directory credentials\n\n    Options:\n      --profile TEXT                  AWS cli profile that will be authenticated.\n                                      After successful authentication just use:\n                                      aws --profile <authenticated profile>\n                                      <service> ...\n      --region TEXT                   The default AWS region that this script will\n                                      connect to for all API calls\n      --ssl-verification / --no-ssl-verification\n                                      SSL certificate verification: Whether or not\n                                      strict certificate verification is done,\n                                      False should only be used for dev/test\n      --adfs-ca-bundle TEXT           Override CA bundle for SSL certificate\n                                      verification for ADFS server only.\n      --adfs-host TEXT                For the first time for a profile it has to\n                                      be provided, next time for the same profile\n                                      it will be loaded from the stored\n                                      configuration\n      --output-format [json|text|table]\n                                      Output format used by aws cli\n      --provider-id TEXT              Provider ID, e.g urn:amazon:webservices\n                                      (optional)\n      --s3-signature-version [s3v4]   s3 signature version: Identifies the version\n                                      of AWS Signature to support for\n                                      authenticated requests. Valid values: s3v4\n      --username-password-command TEXT\n                                      Read username and password from the output\n                                      of a shell command (expected JSON format:\n                                      `{"username": "myusername", "password":\n                                      "mypassword"}`)\n      --env                           Read username, password from environment\n                                      variables (username and password).\n      --stdin                         Read username, password from standard input\n                                      separated by a newline.\n      --authfile TEXT                 Read username, password from a local file\n                                      (optional)\n      --stdout                        Print aws_session_token in json on stdout.\n      --printenv                      Output commands to set AWS_ACCESS_KEY_ID,\n                                      AWS_SECRET_ACCESS_KEY, AWS_SESSION_TOKEN,\n                                      AWS_DEFAULT_REGION environmental variables\n                                      instead of saving them to the aws\n                                      configuration file.\n      --print-console-signin-url      Output a URL that lets users who sign in to\n                                      your organization\'s network securely access\n                                      the AWS Management Console.\n      --console-role-arn TEXT         Role to assume for use in conjunction with\n                                      --print-console-signin-url\n      --console-external-id TEXT      External ID to pass in assume role for use\n                                      in conjunction with --print-console-signin-\n                                      url\n      --role-arn TEXT                 Predefined role arn to selects, e.g. aws-\n                                      adfs login --role-arn arn:aws:iam::123456789\n                                      012:role/YourSpecialRole\n      --session-duration INTEGER      Define the amount of seconds you want to\n                                      establish your STS session, e.g. aws-adfs\n                                      login --session-duration 3600\n      --no-session-cache              Do not use AWS session cache in\n                                      ~/.aws/adfs_cache/ directory.\n      --assertfile TEXT               Use SAML assertion response from a local\n                                      file\n      --sspi / --no-sspi              Whether or not to use Kerberos SSO\n                                      authentication via SSPI (Windows only,\n                                      defaults to True).\n      --duo-factor TEXT               Use a specific Duo factor, overriding the\n                                      default one configured server side. Known\n                                      Duo factors that can be used with aws-adfs\n                                      are "Duo Push", "Passcode", "Phone Call" and\n                                      "WebAuthn Security Key".\n      --duo-device TEXT               Use a specific Duo device, overriding the\n                                      default one configured server side. Depends\n                                      heavily on the Duo factor used. Known Duo\n                                      devices that can be used with aws-adfs are\n                                      "phone1" for "Duo Push" and "Phone Call"\n                                      factors. For "Passcode" and "WebAuthn\n                                      Security Key" factors, it is always "None".\n      --enforce-role-arn              Only allow the role passed in by --role-arn.\n      --aad-verification-code TEXT    Verification code for Azure AD multi-factor\n                                      authentication.\n      --help                          Show this message and exit.\n    ```\n    <!-- AWS_LOGIN_HELP_END -->\n\n    <!-- AWS_RESET_HELP_START -->\n    ```\n    $ aws-adfs reset --help\n    Usage: aws-adfs reset [OPTIONS]\n\n      removes stored profile\n\n    Options:\n      --profile TEXT  AWS cli profile that will be removed\n      --help          Show this message and exit.\n    ```\n    <!-- AWS_RESET_HELP_END -->\n\n## Known issues\n\n* duo-security\n\n    `Error: Cannot begin authentication process. The error response: {"message": "Unknown authentication method.", "stat": "FAIL"}`\n\n    Please setup preferred auth method in duo-security settings (settings\' -> \'My Settings & Devices\').\n\n* USB FIDO2 does not work in Windows Subsystem for Linux (WSL)\n\n    `OSError: [Errno 2] No such file or directory: \'/sys/class/hidraw\'`\n\n    USB devices are not accessible in WSL, please install and run `aws-adfs` on the Windows 10 host and then access the credentials in WSL from the filesystem. Example:\n\n    ```\n    export AWS_CONFIG_FILE=/mnt/c/Users/username/.aws/config\n    export AWS_SHARED_CREDENTIALS_FILE=/mnt/c/Users/username/.aws/credentials\n    ```\n\n*  FIDO2 devices are not detected on Windows 10 build 1903 or newer\n\n    Running `aws-adfs` as Administrator is required since Windows 10 build 1903 to access FIDO2 devices, cf. https://github.com/Yubico/python-fido2/issues/55)\n\n* in cases of trouble with lxml please install\n\n  ```\n  sudo apt-get install python3-dev libxml2-dev libxslt1-dev zlib1g-dev\n  ```\n\n* in cases of trouble with pykerberos please install\n\n  ```\n  sudo apt-get install python3-dev libkrb5-dev\n  ```\n\n* in cases of trouble with OSX Sierra (obsolete OpenSSL), upgrade OpenSSL. Example:\n  ```\n  brew upgrade openssl\n  ```\n  AND add explicit directive to .bash_profile:\n  ```\n  export PATH=$(brew --prefix openssl)/bin:$PATH\n  ```\n\n* only python >= 3.7 to <4.0 are supported:\n  - python 2.6 is not supported\n  - python 2.7 is not supported\n  - python 3.2 is not supported\n  - python 3.3 is not supported\n  - python 3.4 is not supported\n  - python 3.5 is not supported\n  - python 3.6 is not supported\n\n## Development\n\n* update dependencies:\n```\npoetry update\n```\n\n* run unit tests:\n```\npoetry run pytest\n```\n\n* release:\n\n```\nexport CHANGELOG_GITHUB_TOKEN=$(gopass show -o pins/Github/github-changelog-generator)\n./scripts/release.sh patch # or minor, major, prepatch, preminor, premajor, prerelease, or a valid semver string\n```\n\n## Changelog\n\nSee the [CHANGELOG.md](CHANGELOG.md) file, which is generated using [github-changelog-generator](https://github.com/github-changelog-generator/github-changelog-generator).\n',
     'author': 'Venth',
     'author_email': 'artur.krysiak.warszawa@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `aws_adfs-2.7.0/PKG-INFO` & `aws_adfs-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-adfs
-Version: 2.7.0
+Version: 2.8.0
 Summary: AWS CLI authenticator via ADFS - small command-line tool to authenticate via ADFS and assume chosen role
 Keywords: aws,adfs,console,tool
 Author: Venth
 Author-email: artur.krysiak.warszawa@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -416,14 +416,14 @@
 poetry run pytest
 ```
 
 * release:
 
 ```
 export CHANGELOG_GITHUB_TOKEN=$(gopass show -o pins/Github/github-changelog-generator)
-./script/release.sh patch # or minor, major, prepatch, preminor, premajor, prerelease, or a valid semver string
+./scripts/release.sh patch # or minor, major, prepatch, preminor, premajor, prerelease, or a valid semver string
 ```
 
 ## Changelog
 
 See the [CHANGELOG.md](CHANGELOG.md) file, which is generated using [github-changelog-generator](https://github.com/github-changelog-generator/github-changelog-generator).
```

