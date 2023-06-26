# Comparing `tmp/goldbook-0.1.tar.gz` & `tmp/goldbook-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goldbook-0.1.tar", last modified: Mon Feb 28 05:03:01 2022, max compression
+gzip compressed data, was "goldbook-0.2.tar", last modified: Mon Jun 26 18:31:48 2023, max compression
```

## Comparing `goldbook-0.1.tar` & `goldbook-0.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 pdbethke  (1000) pdbethke  (1000)        0 2022-02-28 05:03:01.857239 goldbook-0.1/
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)        0 2022-02-28 04:19:43.000000 goldbook-0.1/LICENSE.txt
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      269 2022-02-28 05:03:01.857239 goldbook-0.1/PKG-INFO
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)        0 2022-02-28 04:20:14.000000 goldbook-0.1/README.md
-drwxrwxr-x   0 pdbethke  (1000) pdbethke  (1000)        0 2022-02-28 05:03:01.857239 goldbook-0.1/goldbook/
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)        0 2022-02-26 23:34:36.000000 goldbook-0.1/goldbook/__init__.py
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)       63 2022-02-26 23:34:36.000000 goldbook-0.1/goldbook/admin.py
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      148 2022-02-26 23:34:36.000000 goldbook-0.1/goldbook/apps.py
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      503 2022-02-26 23:34:36.000000 goldbook-0.1/goldbook/choices.py
-drwxrwxr-x   0 pdbethke  (1000) pdbethke  (1000)        0 2022-02-28 05:03:01.857239 goldbook-0.1/goldbook/migrations/
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)    18070 2022-02-26 23:34:36.000000 goldbook-0.1/goldbook/migrations/0001_initial.py
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)     1432 2022-02-26 23:34:36.000000 goldbook-0.1/goldbook/migrations/0002_winetrail_remove_winery_trail_a_part_of_and_more.py
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)     1359 2022-02-26 23:34:36.000000 goldbook-0.1/goldbook/migrations/0003_ava_alter_winery_ava.py
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      525 2022-02-26 23:34:36.000000 goldbook-0.1/goldbook/migrations/0004_winery_food_truck.py
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      491 2022-02-26 23:34:36.000000 goldbook-0.1/goldbook/migrations/0005_winery_quantity_limit_on_walkin_party_size.py
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)     1396 2022-02-26 23:34:36.000000 goldbook-0.1/goldbook/migrations/0006_viewsfromseating_winery_tastingroom_views.py
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      871 2022-02-26 23:34:36.000000 goldbook-0.1/goldbook/migrations/0007_winery_ceremony_views_and_more.py
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)        0 2022-02-26 23:34:36.000000 goldbook-0.1/goldbook/migrations/__init__.py
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)    34452 2022-02-26 23:34:36.000000 goldbook-0.1/goldbook/models.py
-drwxrwxr-x   0 pdbethke  (1000) pdbethke  (1000)        0 2022-02-28 05:03:01.857239 goldbook-0.1/goldbook/util/
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)        0 2022-02-26 23:34:36.000000 goldbook-0.1/goldbook/util/__init__.py
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      305 2022-02-26 23:34:36.000000 goldbook-0.1/goldbook/util/helpers.py
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)       63 2022-02-26 23:34:36.000000 goldbook-0.1/goldbook/views.py
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      696 2022-02-26 23:34:36.000000 goldbook-0.1/goldbook/wagtail_hooks.py
-drwxrwxr-x   0 pdbethke  (1000) pdbethke  (1000)        0 2022-02-28 05:03:01.857239 goldbook-0.1/goldbook.egg-info/
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      269 2022-02-28 05:03:01.000000 goldbook-0.1/goldbook.egg-info/PKG-INFO
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      819 2022-02-28 05:03:01.000000 goldbook-0.1/goldbook.egg-info/SOURCES.txt
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)        1 2022-02-28 05:03:01.000000 goldbook-0.1/goldbook.egg-info/dependency_links.txt
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)        1 2022-02-28 04:57:40.000000 goldbook-0.1/goldbook.egg-info/not-zip-safe
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)        9 2022-02-28 05:03:01.000000 goldbook-0.1/goldbook.egg-info/top_level.txt
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)       38 2022-02-28 05:03:01.857239 goldbook-0.1/setup.cfg
--rw-rw-r--   0 pdbethke  (1000) pdbethke  (1000)      666 2022-02-28 04:57:33.000000 goldbook-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:31:48.655331 goldbook-0.2/
+-rw-rw-rw-   0        0        0        0 2023-06-21 15:16:30.000000 goldbook-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      292 2023-06-26 18:31:48.655331 goldbook-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-21 15:16:30.000000 goldbook-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 18:31:48.596328 goldbook-0.2/goldbook/
+-rw-rw-rw-   0        0        0        0 2023-06-21 15:16:30.000000 goldbook-0.2/goldbook/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-06-21 15:16:30.000000 goldbook-0.2/goldbook/admin.py
+-rw-rw-rw-   0        0        0      154 2023-06-21 15:16:30.000000 goldbook-0.2/goldbook/apps.py
+-rw-rw-rw-   0        0        0      526 2023-06-21 15:16:30.000000 goldbook-0.2/goldbook/choices.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:31:48.649329 goldbook-0.2/goldbook/migrations/
+-rw-rw-rw-   0        0        0    18197 2023-06-21 15:58:21.000000 goldbook-0.2/goldbook/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1468 2023-06-21 15:16:30.000000 goldbook-0.2/goldbook/migrations/0002_winetrail_remove_winery_trail_a_part_of_and_more.py
+-rw-rw-rw-   0        0        0     1391 2023-06-21 15:16:30.000000 goldbook-0.2/goldbook/migrations/0003_ava_alter_winery_ava.py
+-rw-rw-rw-   0        0        0      544 2023-06-21 15:16:30.000000 goldbook-0.2/goldbook/migrations/0004_winery_food_truck.py
+-rw-rw-rw-   0        0        0      509 2023-06-21 15:16:30.000000 goldbook-0.2/goldbook/migrations/0005_winery_quantity_limit_on_walkin_party_size.py
+-rw-rw-rw-   0        0        0     1428 2023-06-21 15:16:30.000000 goldbook-0.2/goldbook/migrations/0006_viewsfromseating_winery_tastingroom_views.py
+-rw-rw-rw-   0        0        0      895 2023-06-21 15:16:30.000000 goldbook-0.2/goldbook/migrations/0007_winery_ceremony_views_and_more.py
+-rw-rw-rw-   0        0        0     1100 2023-06-21 17:21:44.000000 goldbook-0.2/goldbook/migrations/0008_alter_winery_address_and_more.py
+-rw-rw-rw-   0        0        0        0 2023-06-21 15:16:30.000000 goldbook-0.2/goldbook/migrations/__init__.py
+-rw-rw-rw-   0        0        0    35455 2023-06-21 19:29:46.000000 goldbook-0.2/goldbook/models.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:31:48.654330 goldbook-0.2/goldbook/util/
+-rw-rw-rw-   0        0        0        0 2023-06-21 15:16:30.000000 goldbook-0.2/goldbook/util/__init__.py
+-rw-rw-rw-   0        0        0      316 2023-06-21 15:16:30.000000 goldbook-0.2/goldbook/util/helpers.py
+-rw-rw-rw-   0        0        0       66 2023-06-21 15:16:30.000000 goldbook-0.2/goldbook/views.py
+-rw-rw-rw-   0        0        0      703 2023-06-21 15:50:17.000000 goldbook-0.2/goldbook/wagtail_hooks.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:31:48.606328 goldbook-0.2/goldbook.egg-info/
+-rw-rw-rw-   0        0        0      292 2023-06-26 18:31:48.000000 goldbook-0.2/goldbook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      877 2023-06-26 18:31:48.000000 goldbook-0.2/goldbook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 18:31:48.000000 goldbook-0.2/goldbook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-21 16:31:12.000000 goldbook-0.2/goldbook.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-06-26 18:31:48.000000 goldbook-0.2/goldbook.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 18:31:48.655331 goldbook-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      703 2023-06-21 16:30:59.000000 goldbook-0.2/setup.py
```

### Comparing `goldbook-0.1/goldbook/migrations/0001_initial.py` & `goldbook-0.2/goldbook/migrations/0001_initial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-# Generated by Django 4.0.2 on 2022-02-14 18:24
-
-from django.db import migrations, models
-import django.db.models.deletion
-import goldbook.util.helpers
-import modelcluster.fields
-import phonenumber_field.modelfields
-import wagtail.core.blocks
-import wagtail.core.fields
-import wagtailgeowidget.blocks
-
-
-class Migration(migrations.Migration):
-
-    initial = True
-
-    dependencies = [
-        ('wagtailcore', '0066_collection_management_permissions'),
-        ('wagtailimages', '0023_add_choose_permissions'),
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='Occurrence',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('sort_order', models.IntegerField(blank=True, editable=False, null=True)),
-                ('name', models.CharField(help_text="The name of the Occurrence as you'd like it to be seen by the public", max_length=255, verbose_name='Name')),
-                ('slug', models.SlugField(allow_unicode=True, help_text='The name of the region as it will appear in URLs e.g http://domain.com/wineries/northern-va/', max_length=255, verbose_name='slug')),
-            ],
-            options={
-                'verbose_name': 'Occurrence',
-                'verbose_name_plural': 'Occurrences',
-            },
-        ),
-        migrations.CreateModel(
-            name='WineriesIndexPage',
-            fields=[
-                ('page_ptr', models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, serialize=False, to='wagtailcore.page')),
-            ],
-            options={
-                'verbose_name': 'Wineries',
-                'verbose_name_plural': 'Wineries',
-            },
-            bases=('wagtailcore.page',),
-        ),
-        migrations.CreateModel(
-            name='WineryRegion',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('sort_order', models.IntegerField(blank=True, editable=False, null=True)),
-                ('name', models.CharField(help_text="The name of the Region as you'd like it to be seen by the public", max_length=255, verbose_name='Name')),
-                ('slug', models.SlugField(allow_unicode=True, help_text='The name of the region as it will appear in URLs e.g http://domain.com/wineries/northern-va/', max_length=255, verbose_name='slug')),
-            ],
-            options={
-                'verbose_name': 'Winery Region',
-                'verbose_name_plural': 'Winery Regions',
-            },
-        ),
-        migrations.CreateModel(
-            name='Winery',
-            fields=[
-                ('page_ptr', models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, serialize=False, to='wagtailcore.page')),
-                ('description', wagtail.core.fields.RichTextField(blank=True, null=True)),
-                ('notes', wagtail.core.fields.RichTextField(blank=True, null=True)),
-                ('phone_number', phonenumber_field.modelfields.PhoneNumberField(blank=True, max_length=128, null=True, region=None, verbose_name='Business Phone')),
-                ('email', models.EmailField(blank=True, max_length=254, null=True, verbose_name='Business Email')),
-                ('year_established', models.IntegerField(blank=True, null=True, validators=[goldbook.util.helpers.my_year_validator], verbose_name='Year established')),
-                ('number_of_wines', models.IntegerField(blank=True, null=True, verbose_name='Number of Wines Produced')),
-                ('total_number_wine_cases_annually', models.IntegerField(blank=True, null=True, verbose_name='Total number of cases in production annually')),
-                ('number_of_acres_under_vine', models.IntegerField(blank=True, null=True, verbose_name='Number of acres under vine')),
-                ('ava', models.CharField(blank=True, max_length=254, null=True)),
-                ('trail_a_part_of', models.CharField(blank=True, max_length=254, null=True, verbose_name='Trail a part of')),
-                ('largest_town_within_30_mins', models.CharField(blank=True, max_length=254, null=True, verbose_name='Largest town within 30 min')),
-                ('tasting_room_within_vineyard', models.BooleanField(blank=True, null=True, verbose_name='Is the Tasting Room located within a vineyard?')),
-                ('wine_tours_available', models.BooleanField(blank=True, null=True, verbose_name='Winery tours available?')),
-                ('wines_sold_online', models.BooleanField(blank=True, null=True, verbose_name='Wines sold online?')),
-                ('wine_club', models.BooleanField(blank=True, null=True, verbose_name='Wines Club?')),
-                ('num_wine_club_members', models.IntegerField(blank=True, null=True, verbose_name='Number of Wine Club members?')),
-                ('num_gov_cup_medals', models.IntegerField(blank=True, null=True, verbose_name='Number of Gov Cup Gold medals over the years?')),
-                ('num_other_medals', models.IntegerField(blank=True, null=True, verbose_name='Number of other gold medals of note')),
-                ('primary_contact_name', models.CharField(blank=True, max_length=254, null=True, verbose_name='Primary Contact Name')),
-                ('primary_contact_title', models.CharField(blank=True, max_length=254, null=True, verbose_name='Primary Contact Title')),
-                ('primary_contact_phone', models.CharField(blank=True, max_length=254, null=True, verbose_name='Primary Contact Phone')),
-                ('primary_contact_email', models.CharField(blank=True, max_length=254, null=True, verbose_name='Primary Contact email')),
-                ('secondary_contact_name', models.CharField(blank=True, max_length=254, null=True, verbose_name='Secondary Contact Name')),
-                ('secondary_contact_title', models.CharField(blank=True, max_length=254, null=True, verbose_name='Secondary Contact Title')),
-                ('secondary_contact_phone', models.CharField(blank=True, max_length=254, null=True, verbose_name='Secondary Contact Phone')),
-                ('secondary_contact_email', models.CharField(blank=True, max_length=254, null=True, verbose_name='Secondary Contact email')),
-                ('owner_name', models.CharField(blank=True, max_length=254, null=True, verbose_name='Owner Name')),
-                ('owner_phone', models.CharField(blank=True, max_length=254, null=True, verbose_name='Owner Phone')),
-                ('owner_email', models.CharField(blank=True, max_length=254, null=True, verbose_name='Owner email')),
-                ('owner_bio', wagtail.core.fields.RichTextField(blank=True, null=True, verbose_name='Owner Bio')),
-                ('winemaker_name', models.CharField(blank=True, max_length=254, null=True, verbose_name='Winemaker Name')),
-                ('winemaker_phone', models.CharField(blank=True, max_length=254, null=True, verbose_name='Winemaker Phone')),
-                ('winemaker_email', models.CharField(blank=True, max_length=254, null=True, verbose_name='Winemaker email')),
-                ('winemaker_bio', wagtail.core.fields.RichTextField(blank=True, null=True, verbose_name='Winemaker Bio')),
-                ('brewery', models.BooleanField(blank=True, null=True, verbose_name='Brewery?')),
-                ('veg_garden', models.BooleanField(blank=True, null=True, verbose_name='Vegetable or fruit garden on premise?')),
-                ('flower_garden', models.BooleanField(blank=True, null=True, verbose_name='Formal or flower garden on premise?')),
-                ('bee_apiary', models.BooleanField(blank=True, null=True, verbose_name='Bee apiary on premise?')),
-                ('sheep', models.BooleanField(blank=True, null=True, verbose_name='Sheep on premise?')),
-                ('goats', models.BooleanField(blank=True, null=True, verbose_name='Goats on premise?')),
-                ('chicken', models.BooleanField(blank=True, null=True, verbose_name='Chickens on premise?')),
-                ('cattle', models.BooleanField(blank=True, null=True, verbose_name='Cattle on premise?')),
-                ('horses', models.BooleanField(blank=True, null=True, verbose_name='Horses on premise?')),
-                ('honey', models.BooleanField(blank=True, null=True, verbose_name='honey?')),
-                ('jelly', models.BooleanField(blank=True, null=True, verbose_name='jelly?')),
-                ('cheese', models.BooleanField(blank=True, null=True, verbose_name='cheese?')),
-                ('chocolate', models.BooleanField(blank=True, null=True, verbose_name='chocolate?')),
-                ('other_production', models.CharField(blank=True, max_length=254, null=True, verbose_name='Other?')),
-                ('unique_feature_or_activity', wagtail.core.fields.RichTextField(blank=True, null=True, verbose_name='Uniquely different property feature or activity of note?')),
-                ('fridge_nibbles', models.BooleanField(blank=True, null=True, verbose_name='Refrigerated nibbles?')),
-                ('counter_service_casual_fare', models.BooleanField(blank=True, null=True, verbose_name='Counter service casual fare?')),
-                ('table_service_restaurant', models.BooleanField(blank=True, null=True, verbose_name='Table service restaurant?')),
-                ('fine_dining', models.BooleanField(blank=True, null=True, verbose_name='Fine dining?')),
-                ('outside_picnic_food_welcome', models.BooleanField(blank=True, null=True, verbose_name='Outside picnic food welcome?')),
-                ('tasting_room_style', models.CharField(blank=True, choices=[('Mediterranean', 'Mediterranean'), ('Farmhouse', 'Farmhouse'), ('Old World', 'Old World'), ('Modern Rustic', 'Modern Rustic')], default=None, max_length=20, null=True)),
-                ('seating_capacity', models.IntegerField(blank=True, null=True, verbose_name='Seating Capacity')),
-                ('reservations_available', models.BooleanField(blank=True, null=True, verbose_name='Reservations available?')),
-                ('walk_in_limit', models.BooleanField(blank=True, null=True, verbose_name='Quantity limit on walk-in party size?')),
-                ('dogs_welcome', models.BooleanField(blank=True, null=True, verbose_name='Dogs welcome?')),
-                ('children_welcome', models.BooleanField(blank=True, null=True, verbose_name='Children welcome?')),
-                ('tasting_room_views', models.BooleanField(blank=True, null=True, verbose_name='Views from Tasting Room seating?')),
-                ('tasting_room_views_mountains', models.BooleanField(blank=True, null=True, verbose_name='Mountains?')),
-                ('tasting_room_views_vineyard', models.BooleanField(blank=True, null=True, verbose_name='Vineyard?')),
-                ('tasting_room_views_countryside', models.BooleanField(blank=True, null=True, verbose_name='Countryside?')),
-                ('tasting_room_views_urban', models.BooleanField(blank=True, null=True, verbose_name='Urban Views?')),
-                ('fireplace', models.BooleanField(blank=True, null=True, verbose_name='Fireplace present?')),
-                ('fire_tables', models.BooleanField(blank=True, null=True, verbose_name='Firetables available?')),
-                ('outdoor_heating', models.BooleanField(blank=True, null=True, verbose_name='Outdoor heating available?')),
-                ('shade', models.BooleanField(blank=True, null=True, verbose_name='Is shade abundantly available via umbrellas, porches, pergolas?')),
-                ('lawn', models.BooleanField(blank=True, null=True, verbose_name='Is there a lawn available for picnics and games?')),
-                ('loging', models.BooleanField(blank=True, null=True, verbose_name='Lodging on premise?')),
-                ('souvenirs', models.BooleanField(blank=True, null=True, verbose_name='Souvenir shopping on premise?')),
-                ('festivals', models.BooleanField(blank=True, null=True, verbose_name='Festivals?')),
-                ('festivals_info', models.TextField(blank=True, null=True, verbose_name='Festivals titles and months')),
-                ('dinner_events', models.BooleanField(blank=True, null=True, verbose_name='Dinner events?')),
-                ('dinner_events_info', models.TextField(blank=True, null=True, verbose_name='Dinner event titles & months')),
-                ('classes_or_workshops', models.BooleanField(blank=True, null=True, verbose_name='Classes or workshops?')),
-                ('classes_or_workshops_info', models.TextField(blank=True, null=True, verbose_name='Classes or workshops titles & months')),
-                ('corporate_events', models.BooleanField(blank=True, null=True, verbose_name='Corporate events?')),
-                ('private_party_events', models.BooleanField(blank=True, null=True, verbose_name='Private party events?')),
-                ('minimum_private_party_resv', models.IntegerField(blank=True, null=True, verbose_name='Minimum required for private party reservations')),
-                ('maximum_private_party_resv', models.IntegerField(blank=True, null=True, verbose_name='Maximum required for private party reservations')),
-                ('wedding_events', models.BooleanField(blank=True, null=True, verbose_name='Weddings?')),
-                ('wedding_event_capacity', models.IntegerField(blank=True, null=True, verbose_name='Wedding capacity')),
-                ('wedding_event_avg_per_year', models.IntegerField(blank=True, null=True, verbose_name='Average number of wedding per year')),
-                ('wedding_event_price_range', models.CharField(blank=True, max_length=254, null=True, verbose_name='Average price range of weddings hosted')),
-                ('winery_catering_available', models.BooleanField(blank=True, null=True, verbose_name='Winery provided catering available?')),
-                ('winery_catering_required', models.BooleanField(blank=True, null=True, verbose_name='Winery provided catering Required?')),
-                ('designated_ceremony_site', models.BooleanField(blank=True, null=True, verbose_name='Designated ceremony site?')),
-                ('ceremony_views_mountain', models.BooleanField(blank=True, null=True, verbose_name='Ceremony Mountain Views')),
-                ('ceremony_views_vineyard', models.BooleanField(blank=True, null=True, verbose_name='Ceremony Vineyard Views')),
-                ('ceremony_views_countryside', models.BooleanField(blank=True, null=True, verbose_name='Ceremony Countryside Views')),
-                ('ceremony_views_urban', models.BooleanField(blank=True, null=True, verbose_name='Ceremony Urban Views')),
-                ('designated_reception_hall', models.BooleanField(blank=True, null=True, verbose_name='Designated Reception Hall?')),
-                ('designated_reception_hall_views_mountain', models.BooleanField(blank=True, null=True, verbose_name='Designated Reception Hall Mountain Views')),
-                ('designated_reception_hall_views_vineyard', models.BooleanField(blank=True, null=True, verbose_name='Designated Reception Hall Vineyard Views')),
-                ('designated_reception_hall_views_countryside', models.BooleanField(blank=True, null=True, verbose_name='Designated Reception Hall Countryside Views')),
-                ('designated_reception_hall_views_urban', models.BooleanField(blank=True, null=True, verbose_name='Designated Reception Hall Urban Views')),
-                ('familiar_with_wc_life', models.BooleanField(blank=True, null=True, verbose_name='Are you familiar with Wine & Country Life?')),
-                ('display_wc_life_tasting_room', models.BooleanField(blank=True, null=True, verbose_name='Do you display it in the Tasting Room?')),
-                ('wc_life_advertiser', models.BooleanField(blank=True, null=True, verbose_name='Do you currently advertise in WC.Life?')),
-                ('familiar_with_wc_weddings', models.BooleanField(blank=True, null=True, verbose_name='Are you familiar with Wine & Country Weddings?')),
-                ('display_wc_weddings_tasting_room', models.BooleanField(blank=True, null=True, verbose_name='Do you display it in the Tasting Room?')),
-                ('wc_weddings_advertiser', models.BooleanField(blank=True, null=True, verbose_name='Do you currently advertise in WC.Weddings?')),
-                ('familiar_with_wc_goldbook', models.BooleanField(blank=True, null=True, verbose_name='Are you familiar with The Wine & Country Gold Book?')),
-                ('sell_wc_goldbook', models.BooleanField(blank=True, null=True, verbose_name='Do they currently sell copies of the Gold Book?')),
-                ('wc_goldbook_advertiser', models.BooleanField(blank=True, null=True, verbose_name='Do they currently advertise in WC.Gold Book?')),
-                ('address', wagtail.core.fields.StreamField([('map_struct', wagtail.core.blocks.StructBlock([('address', wagtailgeowidget.blocks.GeoAddressBlock(required=True)), ('map', wagtailgeowidget.blocks.GeoBlock(address_field='address'))]))], blank=True)),
-                ('tasting_room_address', wagtail.core.fields.StreamField([('map_struct', wagtail.core.blocks.StructBlock([('address', wagtailgeowidget.blocks.GeoAddressBlock(required=False)), ('map', wagtailgeowidget.blocks.GeoBlock(address_field='tasting_room_address'))]))], blank=True)),
-                ('live_music', modelcluster.fields.ParentalManyToManyField(blank=True, to='goldbook.Occurrence', verbose_name='Live Music?')),
-                ('logo', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='winery_logo', to='wagtailimages.image')),
-                ('winery_region', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='+', to='goldbook.wineryregion', verbose_name='Region of VA')),
-            ],
-            options={
-                'abstract': False,
-            },
-            bases=('wagtailcore.page',),
-        ),
-    ]
+# Generated by Django 4.0.2 on 2022-02-14 18:24
+
+from django.db import migrations, models
+import django.db.models.deletion
+import goldbook.util.helpers
+import modelcluster.fields
+import phonenumber_field.modelfields
+import wagtail.blocks
+import wagtail.fields
+import wagtailgeowidget.blocks
+
+
+class Migration(migrations.Migration):
+
+    initial = True
+
+    dependencies = [
+        ('wagtailcore', '0066_collection_management_permissions'),
+        ('wagtailimages', '0023_add_choose_permissions'),
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='Occurrence',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('sort_order', models.IntegerField(blank=True, editable=False, null=True)),
+                ('name', models.CharField(help_text="The name of the Occurrence as you'd like it to be seen by the public", max_length=255, verbose_name='Name')),
+                ('slug', models.SlugField(allow_unicode=True, help_text='The name of the region as it will appear in URLs e.g http://domain.com/wineries/northern-va/', max_length=255, verbose_name='slug')),
+            ],
+            options={
+                'verbose_name': 'Occurrence',
+                'verbose_name_plural': 'Occurrences',
+            },
+        ),
+        migrations.CreateModel(
+            name='WineriesIndexPage',
+            fields=[
+                ('page_ptr', models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, serialize=False, to='wagtailcore.page')),
+            ],
+            options={
+                'verbose_name': 'Wineries',
+                'verbose_name_plural': 'Wineries',
+            },
+            bases=('wagtailcore.page',),
+        ),
+        migrations.CreateModel(
+            name='WineryRegion',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('sort_order', models.IntegerField(blank=True, editable=False, null=True)),
+                ('name', models.CharField(help_text="The name of the Region as you'd like it to be seen by the public", max_length=255, verbose_name='Name')),
+                ('slug', models.SlugField(allow_unicode=True, help_text='The name of the region as it will appear in URLs e.g http://domain.com/wineries/northern-va/', max_length=255, verbose_name='slug')),
+            ],
+            options={
+                'verbose_name': 'Winery Region',
+                'verbose_name_plural': 'Winery Regions',
+            },
+        ),
+        migrations.CreateModel(
+            name='Winery',
+            fields=[
+                ('page_ptr', models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, serialize=False, to='wagtailcore.page')),
+                ('description', wagtail.fields.RichTextField(blank=True, null=True)),
+                ('notes', wagtail.fields.RichTextField(blank=True, null=True)),
+                ('phone_number', phonenumber_field.modelfields.PhoneNumberField(blank=True, max_length=128, null=True, region=None, verbose_name='Business Phone')),
+                ('email', models.EmailField(blank=True, max_length=254, null=True, verbose_name='Business Email')),
+                ('year_established', models.IntegerField(blank=True, null=True, validators=[goldbook.util.helpers.my_year_validator], verbose_name='Year established')),
+                ('number_of_wines', models.IntegerField(blank=True, null=True, verbose_name='Number of Wines Produced')),
+                ('total_number_wine_cases_annually', models.IntegerField(blank=True, null=True, verbose_name='Total number of cases in production annually')),
+                ('number_of_acres_under_vine', models.IntegerField(blank=True, null=True, verbose_name='Number of acres under vine')),
+                ('ava', models.CharField(blank=True, max_length=254, null=True)),
+                ('trail_a_part_of', models.CharField(blank=True, max_length=254, null=True, verbose_name='Trail a part of')),
+                ('largest_town_within_30_mins', models.CharField(blank=True, max_length=254, null=True, verbose_name='Largest town within 30 min')),
+                ('tasting_room_within_vineyard', models.BooleanField(blank=True, null=True, verbose_name='Is the Tasting Room located within a vineyard?')),
+                ('wine_tours_available', models.BooleanField(blank=True, null=True, verbose_name='Winery tours available?')),
+                ('wines_sold_online', models.BooleanField(blank=True, null=True, verbose_name='Wines sold online?')),
+                ('wine_club', models.BooleanField(blank=True, null=True, verbose_name='Wines Club?')),
+                ('num_wine_club_members', models.IntegerField(blank=True, null=True, verbose_name='Number of Wine Club members?')),
+                ('num_gov_cup_medals', models.IntegerField(blank=True, null=True, verbose_name='Number of Gov Cup Gold medals over the years?')),
+                ('num_other_medals', models.IntegerField(blank=True, null=True, verbose_name='Number of other gold medals of note')),
+                ('primary_contact_name', models.CharField(blank=True, max_length=254, null=True, verbose_name='Primary Contact Name')),
+                ('primary_contact_title', models.CharField(blank=True, max_length=254, null=True, verbose_name='Primary Contact Title')),
+                ('primary_contact_phone', models.CharField(blank=True, max_length=254, null=True, verbose_name='Primary Contact Phone')),
+                ('primary_contact_email', models.CharField(blank=True, max_length=254, null=True, verbose_name='Primary Contact email')),
+                ('secondary_contact_name', models.CharField(blank=True, max_length=254, null=True, verbose_name='Secondary Contact Name')),
+                ('secondary_contact_title', models.CharField(blank=True, max_length=254, null=True, verbose_name='Secondary Contact Title')),
+                ('secondary_contact_phone', models.CharField(blank=True, max_length=254, null=True, verbose_name='Secondary Contact Phone')),
+                ('secondary_contact_email', models.CharField(blank=True, max_length=254, null=True, verbose_name='Secondary Contact email')),
+                ('owner_name', models.CharField(blank=True, max_length=254, null=True, verbose_name='Owner Name')),
+                ('owner_phone', models.CharField(blank=True, max_length=254, null=True, verbose_name='Owner Phone')),
+                ('owner_email', models.CharField(blank=True, max_length=254, null=True, verbose_name='Owner email')),
+                ('owner_bio', wagtail.fields.RichTextField(blank=True, null=True, verbose_name='Owner Bio')),
+                ('winemaker_name', models.CharField(blank=True, max_length=254, null=True, verbose_name='Winemaker Name')),
+                ('winemaker_phone', models.CharField(blank=True, max_length=254, null=True, verbose_name='Winemaker Phone')),
+                ('winemaker_email', models.CharField(blank=True, max_length=254, null=True, verbose_name='Winemaker email')),
+                ('winemaker_bio', wagtail.fields.RichTextField(blank=True, null=True, verbose_name='Winemaker Bio')),
+                ('brewery', models.BooleanField(blank=True, null=True, verbose_name='Brewery?')),
+                ('veg_garden', models.BooleanField(blank=True, null=True, verbose_name='Vegetable or fruit garden on premise?')),
+                ('flower_garden', models.BooleanField(blank=True, null=True, verbose_name='Formal or flower garden on premise?')),
+                ('bee_apiary', models.BooleanField(blank=True, null=True, verbose_name='Bee apiary on premise?')),
+                ('sheep', models.BooleanField(blank=True, null=True, verbose_name='Sheep on premise?')),
+                ('goats', models.BooleanField(blank=True, null=True, verbose_name='Goats on premise?')),
+                ('chicken', models.BooleanField(blank=True, null=True, verbose_name='Chickens on premise?')),
+                ('cattle', models.BooleanField(blank=True, null=True, verbose_name='Cattle on premise?')),
+                ('horses', models.BooleanField(blank=True, null=True, verbose_name='Horses on premise?')),
+                ('honey', models.BooleanField(blank=True, null=True, verbose_name='honey?')),
+                ('jelly', models.BooleanField(blank=True, null=True, verbose_name='jelly?')),
+                ('cheese', models.BooleanField(blank=True, null=True, verbose_name='cheese?')),
+                ('chocolate', models.BooleanField(blank=True, null=True, verbose_name='chocolate?')),
+                ('other_production', models.CharField(blank=True, max_length=254, null=True, verbose_name='Other?')),
+                ('unique_feature_or_activity', wagtail.fields.RichTextField(blank=True, null=True, verbose_name='Uniquely different property feature or activity of note?')),
+                ('fridge_nibbles', models.BooleanField(blank=True, null=True, verbose_name='Refrigerated nibbles?')),
+                ('counter_service_casual_fare', models.BooleanField(blank=True, null=True, verbose_name='Counter service casual fare?')),
+                ('table_service_restaurant', models.BooleanField(blank=True, null=True, verbose_name='Table service restaurant?')),
+                ('fine_dining', models.BooleanField(blank=True, null=True, verbose_name='Fine dining?')),
+                ('outside_picnic_food_welcome', models.BooleanField(blank=True, null=True, verbose_name='Outside picnic food welcome?')),
+                ('tasting_room_style', models.CharField(blank=True, choices=[('Mediterranean', 'Mediterranean'), ('Farmhouse', 'Farmhouse'), ('Old World', 'Old World'), ('Modern Rustic', 'Modern Rustic')], default=None, max_length=20, null=True)),
+                ('seating_capacity', models.IntegerField(blank=True, null=True, verbose_name='Seating Capacity')),
+                ('reservations_available', models.BooleanField(blank=True, null=True, verbose_name='Reservations available?')),
+                ('walk_in_limit', models.BooleanField(blank=True, null=True, verbose_name='Quantity limit on walk-in party size?')),
+                ('dogs_welcome', models.BooleanField(blank=True, null=True, verbose_name='Dogs welcome?')),
+                ('children_welcome', models.BooleanField(blank=True, null=True, verbose_name='Children welcome?')),
+                ('tasting_room_views', models.BooleanField(blank=True, null=True, verbose_name='Views from Tasting Room seating?')),
+                ('tasting_room_views_mountains', models.BooleanField(blank=True, null=True, verbose_name='Mountains?')),
+                ('tasting_room_views_vineyard', models.BooleanField(blank=True, null=True, verbose_name='Vineyard?')),
+                ('tasting_room_views_countryside', models.BooleanField(blank=True, null=True, verbose_name='Countryside?')),
+                ('tasting_room_views_urban', models.BooleanField(blank=True, null=True, verbose_name='Urban Views?')),
+                ('fireplace', models.BooleanField(blank=True, null=True, verbose_name='Fireplace present?')),
+                ('fire_tables', models.BooleanField(blank=True, null=True, verbose_name='Firetables available?')),
+                ('outdoor_heating', models.BooleanField(blank=True, null=True, verbose_name='Outdoor heating available?')),
+                ('shade', models.BooleanField(blank=True, null=True, verbose_name='Is shade abundantly available via umbrellas, porches, pergolas?')),
+                ('lawn', models.BooleanField(blank=True, null=True, verbose_name='Is there a lawn available for picnics and games?')),
+                ('loging', models.BooleanField(blank=True, null=True, verbose_name='Lodging on premise?')),
+                ('souvenirs', models.BooleanField(blank=True, null=True, verbose_name='Souvenir shopping on premise?')),
+                ('festivals', models.BooleanField(blank=True, null=True, verbose_name='Festivals?')),
+                ('festivals_info', models.TextField(blank=True, null=True, verbose_name='Festivals titles and months')),
+                ('dinner_events', models.BooleanField(blank=True, null=True, verbose_name='Dinner events?')),
+                ('dinner_events_info', models.TextField(blank=True, null=True, verbose_name='Dinner event titles & months')),
+                ('classes_or_workshops', models.BooleanField(blank=True, null=True, verbose_name='Classes or workshops?')),
+                ('classes_or_workshops_info', models.TextField(blank=True, null=True, verbose_name='Classes or workshops titles & months')),
+                ('corporate_events', models.BooleanField(blank=True, null=True, verbose_name='Corporate events?')),
+                ('private_party_events', models.BooleanField(blank=True, null=True, verbose_name='Private party events?')),
+                ('minimum_private_party_resv', models.IntegerField(blank=True, null=True, verbose_name='Minimum required for private party reservations')),
+                ('maximum_private_party_resv', models.IntegerField(blank=True, null=True, verbose_name='Maximum required for private party reservations')),
+                ('wedding_events', models.BooleanField(blank=True, null=True, verbose_name='Weddings?')),
+                ('wedding_event_capacity', models.IntegerField(blank=True, null=True, verbose_name='Wedding capacity')),
+                ('wedding_event_avg_per_year', models.IntegerField(blank=True, null=True, verbose_name='Average number of wedding per year')),
+                ('wedding_event_price_range', models.CharField(blank=True, max_length=254, null=True, verbose_name='Average price range of weddings hosted')),
+                ('winery_catering_available', models.BooleanField(blank=True, null=True, verbose_name='Winery provided catering available?')),
+                ('winery_catering_required', models.BooleanField(blank=True, null=True, verbose_name='Winery provided catering Required?')),
+                ('designated_ceremony_site', models.BooleanField(blank=True, null=True, verbose_name='Designated ceremony site?')),
+                ('ceremony_views_mountain', models.BooleanField(blank=True, null=True, verbose_name='Ceremony Mountain Views')),
+                ('ceremony_views_vineyard', models.BooleanField(blank=True, null=True, verbose_name='Ceremony Vineyard Views')),
+                ('ceremony_views_countryside', models.BooleanField(blank=True, null=True, verbose_name='Ceremony Countryside Views')),
+                ('ceremony_views_urban', models.BooleanField(blank=True, null=True, verbose_name='Ceremony Urban Views')),
+                ('designated_reception_hall', models.BooleanField(blank=True, null=True, verbose_name='Designated Reception Hall?')),
+                ('designated_reception_hall_views_mountain', models.BooleanField(blank=True, null=True, verbose_name='Designated Reception Hall Mountain Views')),
+                ('designated_reception_hall_views_vineyard', models.BooleanField(blank=True, null=True, verbose_name='Designated Reception Hall Vineyard Views')),
+                ('designated_reception_hall_views_countryside', models.BooleanField(blank=True, null=True, verbose_name='Designated Reception Hall Countryside Views')),
+                ('designated_reception_hall_views_urban', models.BooleanField(blank=True, null=True, verbose_name='Designated Reception Hall Urban Views')),
+                ('familiar_with_wc_life', models.BooleanField(blank=True, null=True, verbose_name='Are you familiar with Wine & Country Life?')),
+                ('display_wc_life_tasting_room', models.BooleanField(blank=True, null=True, verbose_name='Do you display it in the Tasting Room?')),
+                ('wc_life_advertiser', models.BooleanField(blank=True, null=True, verbose_name='Do you currently advertise in WC.Life?')),
+                ('familiar_with_wc_weddings', models.BooleanField(blank=True, null=True, verbose_name='Are you familiar with Wine & Country Weddings?')),
+                ('display_wc_weddings_tasting_room', models.BooleanField(blank=True, null=True, verbose_name='Do you display it in the Tasting Room?')),
+                ('wc_weddings_advertiser', models.BooleanField(blank=True, null=True, verbose_name='Do you currently advertise in WC.Weddings?')),
+                ('familiar_with_wc_goldbook', models.BooleanField(blank=True, null=True, verbose_name='Are you familiar with The Wine & Country Gold Book?')),
+                ('sell_wc_goldbook', models.BooleanField(blank=True, null=True, verbose_name='Do they currently sell copies of the Gold Book?')),
+                ('wc_goldbook_advertiser', models.BooleanField(blank=True, null=True, verbose_name='Do they currently advertise in WC.Gold Book?')),
+                ('address', wagtail.fields.StreamField([('map_struct', wagtail.blocks.StructBlock([('address', wagtailgeowidget.blocks.GeoAddressBlock(required=True)), ('map', wagtailgeowidget.blocks.GeoBlock(address_field='address'))]))], blank=True)),
+                ('tasting_room_address', wagtail.fields.StreamField([('map_struct', wagtail.blocks.StructBlock([('address', wagtailgeowidget.blocks.GeoAddressBlock(required=False)), ('map', wagtailgeowidget.blocks.GeoBlock(address_field='tasting_room_address'))]))], blank=True)),
+                ('live_music', modelcluster.fields.ParentalManyToManyField(blank=True, to='goldbook.Occurrence', verbose_name='Live Music?')),
+                ('logo', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='winery_logo', to='wagtailimages.image')),
+                ('winery_region', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='+', to='goldbook.wineryregion', verbose_name='Region of VA')),
+            ],
+            options={
+                'abstract': False,
+            },
+            bases=('wagtailcore.page',),
+        ),
+    ]
```

### Comparing `goldbook-0.1/goldbook/migrations/0002_winetrail_remove_winery_trail_a_part_of_and_more.py` & `goldbook-0.2/goldbook/migrations/0002_winetrail_remove_winery_trail_a_part_of_and_more.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# Generated by Django 4.0.2 on 2022-02-14 18:45
-
-from django.db import migrations, models
-import modelcluster.fields
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('goldbook', '0001_initial'),
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='WineTrail',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('sort_order', models.IntegerField(blank=True, editable=False, null=True)),
-                ('name', models.CharField(help_text="The name of the Wine Trail as you'd like it to be seen by the public", max_length=255, verbose_name='Name')),
-                ('slug', models.SlugField(allow_unicode=True, help_text='The name of the Wine Trail  as it will appear in URLs e.g http://domain.com/wineries/pub-crawl/', max_length=255, verbose_name='slug')),
-            ],
-            options={
-                'verbose_name': 'Wine Trail',
-                'verbose_name_plural': 'Wine Trails',
-            },
-        ),
-        migrations.RemoveField(
-            model_name='winery',
-            name='trail_a_part_of',
-        ),
-        migrations.AddField(
-            model_name='winery',
-            name='trail_a_part_of',
-            field=modelcluster.fields.ParentalManyToManyField(blank=True, to='goldbook.WineTrail', verbose_name='Trail a part of'),
-        ),
-    ]
+# Generated by Django 4.0.2 on 2022-02-14 18:45
+
+from django.db import migrations, models
+import modelcluster.fields
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ('goldbook', '0001_initial'),
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='WineTrail',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('sort_order', models.IntegerField(blank=True, editable=False, null=True)),
+                ('name', models.CharField(help_text="The name of the Wine Trail as you'd like it to be seen by the public", max_length=255, verbose_name='Name')),
+                ('slug', models.SlugField(allow_unicode=True, help_text='The name of the Wine Trail  as it will appear in URLs e.g http://domain.com/wineries/pub-crawl/', max_length=255, verbose_name='slug')),
+            ],
+            options={
+                'verbose_name': 'Wine Trail',
+                'verbose_name_plural': 'Wine Trails',
+            },
+        ),
+        migrations.RemoveField(
+            model_name='winery',
+            name='trail_a_part_of',
+        ),
+        migrations.AddField(
+            model_name='winery',
+            name='trail_a_part_of',
+            field=modelcluster.fields.ParentalManyToManyField(blank=True, to='goldbook.WineTrail', verbose_name='Trail a part of'),
+        ),
+    ]
```

### Comparing `goldbook-0.1/goldbook/migrations/0003_ava_alter_winery_ava.py` & `goldbook-0.2/goldbook/migrations/0003_ava_alter_winery_ava.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# Generated by Django 4.0.2 on 2022-02-14 18:56
-
-from django.db import migrations, models
-import django.db.models.deletion
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('goldbook', '0002_winetrail_remove_winery_trail_a_part_of_and_more'),
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='AVA',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('sort_order', models.IntegerField(blank=True, editable=False, null=True)),
-                ('name', models.CharField(help_text="The name of the AVA as you'd like it to be seen by the public", max_length=255, verbose_name='Name')),
-                ('slug', models.SlugField(allow_unicode=True, help_text='The name of the AVA  as it will appear in URLs e.g http://domain.com/wineries/ava/blue-ridge/', max_length=255, verbose_name='slug')),
-            ],
-            options={
-                'verbose_name': 'AVA',
-                'verbose_name_plural': 'AVAs',
-            },
-        ),
-        migrations.AlterField(
-            model_name='winery',
-            name='ava',
-            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='+', to='goldbook.ava', verbose_name='AVA'),
-        ),
-    ]
+# Generated by Django 4.0.2 on 2022-02-14 18:56
+
+from django.db import migrations, models
+import django.db.models.deletion
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ('goldbook', '0002_winetrail_remove_winery_trail_a_part_of_and_more'),
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='AVA',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('sort_order', models.IntegerField(blank=True, editable=False, null=True)),
+                ('name', models.CharField(help_text="The name of the AVA as you'd like it to be seen by the public", max_length=255, verbose_name='Name')),
+                ('slug', models.SlugField(allow_unicode=True, help_text='The name of the AVA  as it will appear in URLs e.g http://domain.com/wineries/ava/blue-ridge/', max_length=255, verbose_name='slug')),
+            ],
+            options={
+                'verbose_name': 'AVA',
+                'verbose_name_plural': 'AVAs',
+            },
+        ),
+        migrations.AlterField(
+            model_name='winery',
+            name='ava',
+            field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='+', to='goldbook.ava', verbose_name='AVA'),
+        ),
+    ]
```

### Comparing `goldbook-0.1/goldbook/migrations/0004_winery_food_truck.py` & `goldbook-0.2/goldbook/migrations/0004_winery_food_truck.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# Generated by Django 4.0.2 on 2022-02-17 19:45
-
-from django.db import migrations
-import modelcluster.fields
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('goldbook', '0003_ava_alter_winery_ava'),
-    ]
-
-    operations = [
-        migrations.AddField(
-            model_name='winery',
-            name='food_truck',
-            field=modelcluster.fields.ParentalManyToManyField(blank=True, related_name='food_truck', to='goldbook.Occurrence', verbose_name='Food Truck Available?'),
-        ),
-    ]
+# Generated by Django 4.0.2 on 2022-02-17 19:45
+
+from django.db import migrations
+import modelcluster.fields
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ('goldbook', '0003_ava_alter_winery_ava'),
+    ]
+
+    operations = [
+        migrations.AddField(
+            model_name='winery',
+            name='food_truck',
+            field=modelcluster.fields.ParentalManyToManyField(blank=True, related_name='food_truck', to='goldbook.Occurrence', verbose_name='Food Truck Available?'),
+        ),
+    ]
```

### Comparing `goldbook-0.1/goldbook/migrations/0006_viewsfromseating_winery_tastingroom_views.py` & `goldbook-0.2/goldbook/migrations/0006_viewsfromseating_winery_tastingroom_views.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# Generated by Django 4.0.2 on 2022-02-17 20:25
-
-from django.db import migrations, models
-import modelcluster.fields
-
-
-class Migration(migrations.Migration):
-
-    dependencies = [
-        ('goldbook', '0005_winery_quantity_limit_on_walkin_party_size'),
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='ViewsFromSeating',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('sort_order', models.IntegerField(blank=True, editable=False, null=True)),
-                ('name', models.CharField(help_text="The name of the View as you'd like it to be seen by the public", max_length=255, verbose_name='Name')),
-                ('slug', models.SlugField(allow_unicode=True, help_text='The name of the view as it will appear in URLs e.g http://domain.com/wineries/northern-va/lakeviews/', max_length=255, verbose_name='slug')),
-            ],
-            options={
-                'verbose_name': 'View From Seating',
-                'verbose_name_plural': 'Seating Views',
-            },
-        ),
-        migrations.AddField(
-            model_name='winery',
-            name='tastingroom_views',
-            field=modelcluster.fields.ParentalManyToManyField(blank=True, to='goldbook.ViewsFromSeating', verbose_name='Views from Tasting Room seating?'),
-        ),
-    ]
+# Generated by Django 4.0.2 on 2022-02-17 20:25
+
+from django.db import migrations, models
+import modelcluster.fields
+
+
+class Migration(migrations.Migration):
+
+    dependencies = [
+        ('goldbook', '0005_winery_quantity_limit_on_walkin_party_size'),
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='ViewsFromSeating',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('sort_order', models.IntegerField(blank=True, editable=False, null=True)),
+                ('name', models.CharField(help_text="The name of the View as you'd like it to be seen by the public", max_length=255, verbose_name='Name')),
+                ('slug', models.SlugField(allow_unicode=True, help_text='The name of the view as it will appear in URLs e.g http://domain.com/wineries/northern-va/lakeviews/', max_length=255, verbose_name='slug')),
+            ],
+            options={
+                'verbose_name': 'View From Seating',
+                'verbose_name_plural': 'Seating Views',
+            },
+        ),
+        migrations.AddField(
+            model_name='winery',
+            name='tastingroom_views',
+            field=modelcluster.fields.ParentalManyToManyField(blank=True, to='goldbook.ViewsFromSeating', verbose_name='Views from Tasting Room seating?'),
+        ),
+    ]
```

### Comparing `goldbook-0.1/goldbook/models.py` & `goldbook-0.2/goldbook/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,795 +1,807 @@
-import datetime
-
-from django.db import models
-from django import forms
-from django.utils.translation import gettext_lazy as _
-from django.conf import settings
-from django.core.exceptions import ValidationError
-
-from modelcluster.fields import ParentalKey
-from modelcluster.models import ClusterableModel
-
-from wagtail.core.models import Page, Orderable
-from wagtail.admin.edit_handlers import (
-    FieldPanel,
-    MultiFieldPanel,
-    FieldRowPanel,
-    StreamFieldPanel,
-    InlinePanel,
-    PageChooserPanel,
-    ObjectList,
-    TabbedInterface,
-)
-from wagtail.images.edit_handlers import ImageChooserPanel
-from wagtail.search import index
-from wagtail.core.fields import StreamField, RichTextField
-from wagtail.core import blocks
-from wagtail.snippets.models import register_snippet
-from wagtailgeowidget.blocks import GeoBlock, GeoAddressBlock
-from modelcluster.fields import ParentalManyToManyField
-from phonenumber_field.modelfields import PhoneNumberField
-
-from goldbook.choices import DAY_CHOICES, CONTACT_TYPE_CHOICES, TASTING_ROOM_STYLE
-from goldbook.util.helpers import my_year_validator
-
-
-@register_snippet
-class Occurrence(Orderable):
-    name = models.CharField(
-        verbose_name=_('Name'),
-        max_length=255,
-        help_text=_("The name of the Occurrence as you'd like it to be seen by the public")
-    )
-    slug = models.SlugField(
-        verbose_name=_('slug'),
-        allow_unicode=True,
-        max_length=255,
-        help_text=_("The name of the region as it will appear in URLs e.g http://domain.com/wineries/northern-va/")
-    )
-
-    class Meta:
-        verbose_name = 'Occurrence'
-        verbose_name_plural = 'Occurrences'
-
-    def __str__(self):
-        return self.name
-
-    panels = [
-        FieldPanel('name'),
-        FieldPanel('slug'),
-    ]
-
-@register_snippet
-class WineTrail(Orderable):
-    name = models.CharField(
-        verbose_name=_('Name'),
-        max_length=255,
-        help_text=_("The name of the Wine Trail as you'd like it to be seen by the public")
-    )
-    slug = models.SlugField(
-        verbose_name=_('slug'),
-        allow_unicode=True,
-        max_length=255,
-        help_text=_("The name of the Wine Trail  as it will appear in URLs e.g http://domain.com/wineries/pub-crawl/")
-    )
-
-    class Meta:
-        verbose_name = 'Wine Trail'
-        verbose_name_plural = 'Wine Trails'
-
-    def __str__(self):
-        return self.name
-
-    panels = [
-        FieldPanel('name'),
-        FieldPanel('slug'),
-    ]
-
-
-@register_snippet
-class AVA(Orderable):
-    name = models.CharField(
-        verbose_name=_('Name'),
-        max_length=255,
-        help_text=_("The name of the AVA as you'd like it to be seen by the public")
-    )
-    slug = models.SlugField(
-        verbose_name=_('slug'),
-        allow_unicode=True,
-        max_length=255,
-        help_text=_("The name of the AVA  as it will appear in URLs e.g http://domain.com/wineries/ava/blue-ridge/")
-    )
-
-    class Meta:
-        verbose_name = 'AVA'
-        verbose_name_plural = 'AVAs'
-
-    def __str__(self):
-        return self.name
-
-    panels = [
-        FieldPanel('name'),
-        FieldPanel('slug'),
-    ]
-# class OperatingHours(models.Model):
-#     """
-#     A Django model to capture operating hours for a Location
-#     """
-#
-#     day = models.CharField(
-#         max_length=4,
-#         choices=DAY_CHOICES,
-#         default='MON'
-#     )
-#     opening_time = models.TimeField(
-#         blank=True,
-#         null=True
-#     )
-#     closing_time = models.TimeField(
-#         blank=True,
-#         null=True
-#     )
-#     closed = models.BooleanField(
-#         "Closed?",
-#         blank=True,
-#         help_text='Tick if location is closed on this day'
-#     )
-#
-#     panels = [
-#         FieldPanel('day'),
-#         FieldPanel('opening_time'),
-#         FieldPanel('closing_time'),
-#         FieldPanel('closed'),
-#     ]
-#
-#     class Meta:
-#         abstract = True
-#
-#     def __str__(self):
-#         if self.opening_time:
-#             opening = self.opening_time.strftime('%H:%M')
-#         else:
-#             opening = '--'
-#         if self.closing_time:
-#             closed = self.closing_time.strftime('%H:%M')
-#         else:
-#             closed = '--'
-#         return '{}: {} - {} {}'.format(
-#             self.day,
-#             opening,
-#             closed,
-#             settings.TIME_ZONE
-#         )
-#
-#
-# class WineryOperatingHours(Orderable, OperatingHours):
-#     """
-#     A model creating a relationship between the OperatingHours and Location
-#     Note that unlike BlogPeopleRelationship we don't include a ForeignKey to
-#     OperatingHours as we don't need that relationship (e.g. any Location open
-#     a certain day of the week). The ParentalKey is the minimum required to
-#     relate the two objects to one another. We use the ParentalKey's related_
-#     name to access it from the LocationPage admin
-#     """
-#     location = ParentalKey(
-#         'WineryOld',
-#         related_name='hours_of_operation',
-#         on_delete=models.CASCADE
-#     )
-
-@register_snippet
-class WineryRegion(Orderable):
-    name = models.CharField(
-        verbose_name=_('Name'),
-        max_length=255,
-        help_text=_("The name of the Region as you'd like it to be seen by the public")
-    )
-    slug = models.SlugField(
-        verbose_name=_('slug'),
-        allow_unicode=True,
-        max_length=255,
-        help_text=_("The name of the region as it will appear in URLs e.g http://domain.com/wineries/northern-va/")
-    )
-
-    class Meta:
-        verbose_name = 'Winery Region'
-        verbose_name_plural = 'Winery Regions'
-
-    def __str__(self):
-        return self.name
-
-    panels = [
-        FieldPanel('name'),
-        FieldPanel('slug'),
-    ]
-
-@register_snippet
-class ViewsFromSeating(Orderable):
-    name = models.CharField(
-        verbose_name=_('Name'),
-        max_length=255,
-        help_text=_("The name of the View as you'd like it to be seen by the public")
-    )
-    slug = models.SlugField(
-        verbose_name=_('slug'),
-        allow_unicode=True,
-        max_length=255,
-        help_text=_("The name of the view as it will appear in URLs e.g http://domain.com/wineries/northern-va/lakeviews/")
-    )
-
-    class Meta:
-        verbose_name = 'View From Seating'
-        verbose_name_plural = 'Seating Views'
-
-    def __str__(self):
-        return self.name
-
-    panels = [
-        FieldPanel('name'),
-        FieldPanel('slug'),
-    ]
-
-class WineriesIndexPage(Page):
-    template = 'goldbook/wineries_page.html'
-    max_count = 1
-    subpage_types = [
-        'goldbook.Winery',  # appname.ModelName
-    ]
-
-    class Meta:
-        verbose_name_plural = 'Wineries'
-        verbose_name = 'Wineries'
-
-
-class Winery(Page):
-    subpage_types = []
-    description = RichTextField(null=True, blank=True)
-    notes = RichTextField(null=True, blank=True)
-    phone_number = PhoneNumberField(blank=True, null=True, verbose_name='Business Phone')
-    email = models.EmailField(max_length=254, blank=True, null=True, verbose_name='Business Email')
-    year_established = models.IntegerField(validators=[my_year_validator], blank=True, null=True,
-                                           verbose_name='Year established')
-    number_of_wines = models.IntegerField(blank=True, null=True, verbose_name='Number of Wines Produced')
-    total_number_wine_cases_annually = models.IntegerField(blank=True, null=True,
-                                                           verbose_name='Total number of cases in production annually')
-    number_of_acres_under_vine = models.IntegerField(blank=True, null=True, verbose_name='Number of acres under vine')
-    winery_region = models.ForeignKey('goldbook.WineryRegion', null=True, blank=True, on_delete=models.SET_NULL,
-                                      verbose_name='Region of VA', related_name='+')
-    ava =  models.ForeignKey('goldbook.AVA', blank=True, null=True,  on_delete=models.SET_NULL,
-                                      verbose_name='AVA', related_name='+')
-    trail_a_part_of = ParentalManyToManyField("goldbook.WineTrail", blank=True, verbose_name='Trail a part of')
-    largest_town_within_30_mins = models.CharField(max_length=254, blank=True, null=True,
-                                                   verbose_name='Largest town within 30 min')
-    tasting_room_within_vineyard = models.BooleanField(blank=True, null=True,
-                                                       verbose_name='Is the Tasting Room located within a vineyard?')
-    wine_tours_available = models.BooleanField(blank=True, null=True, verbose_name='Winery tours available?')
-    wines_sold_online = models.BooleanField(blank=True, null=True, verbose_name='Wines sold online?')
-    wine_club = models.BooleanField(blank=True, null=True, verbose_name='Wines Club?')
-    num_wine_club_members = models.IntegerField(blank=True, null=True, verbose_name='Number of Wine Club members?')
-    num_gov_cup_medals = models.IntegerField(blank=True, null=True,
-                                             verbose_name='Number of Gov Cup Gold medals over the years?')
-    num_other_medals = models.IntegerField(blank=True, null=True, verbose_name='Number of other gold medals of note')
-
-    primary_contact_name = models.CharField(max_length=254, blank=True, null=True, verbose_name='Primary Contact Name')
-    primary_contact_title = models.CharField(max_length=254, blank=True, null=True,
-                                             verbose_name='Primary Contact Title')
-    primary_contact_phone = models.CharField(max_length=254, blank=True, null=True,
-                                             verbose_name='Primary Contact Phone')
-    primary_contact_email = models.CharField(max_length=254, blank=True, null=True,
-                                             verbose_name='Primary Contact email')
-    secondary_contact_name = models.CharField(max_length=254, blank=True, null=True,
-                                              verbose_name='Secondary Contact Name')
-    secondary_contact_title = models.CharField(max_length=254, blank=True, null=True,
-                                               verbose_name='Secondary Contact Title')
-    secondary_contact_phone = models.CharField(max_length=254, blank=True, null=True,
-                                               verbose_name='Secondary Contact Phone')
-    secondary_contact_email = models.CharField(max_length=254, blank=True, null=True,
-                                               verbose_name='Secondary Contact email')
-    owner_name = models.CharField(max_length=254, blank=True, null=True,
-                                  verbose_name='Owner Name')
-    owner_phone = models.CharField(max_length=254, blank=True, null=True,
-                                   verbose_name='Owner Phone')
-    owner_email = models.CharField(max_length=254, blank=True, null=True,
-                                   verbose_name='Owner email')
-    owner_bio = RichTextField(null=True, blank=True, verbose_name='Owner Bio')
-    winemaker_name = models.CharField(max_length=254, blank=True, null=True,
-                                      verbose_name='Winemaker Name')
-    winemaker_phone = models.CharField(max_length=254, blank=True, null=True,
-                                       verbose_name='Winemaker Phone')
-    winemaker_email = models.CharField(max_length=254, blank=True, null=True,
-                                       verbose_name='Winemaker email')
-    winemaker_bio = RichTextField(null=True, blank=True, verbose_name='Winemaker Bio')
-    brewery = models.BooleanField(blank=True, null=True, verbose_name='Brewery?')
-    veg_garden = models.BooleanField(blank=True, null=True, verbose_name='Vegetable or fruit garden on premise?')
-    flower_garden = models.BooleanField(blank=True, null=True, verbose_name='Formal or flower garden on premise?')
-    bee_apiary = models.BooleanField(blank=True, null=True, verbose_name='Bee apiary on premise?')
-    sheep = models.BooleanField(blank=True, null=True, verbose_name='Sheep on premise?')
-    goats = models.BooleanField(blank=True, null=True, verbose_name='Goats on premise?')
-    chicken = models.BooleanField(blank=True, null=True, verbose_name='Chickens on premise?')
-    cattle = models.BooleanField(blank=True, null=True, verbose_name='Cattle on premise?')
-    horses = models.BooleanField(blank=True, null=True, verbose_name='Horses on premise?')
-    honey = models.BooleanField(blank=True, null=True, verbose_name='honey?')
-    jelly = models.BooleanField(blank=True, null=True, verbose_name='jelly?')
-    cheese = models.BooleanField(blank=True, null=True, verbose_name='cheese?')
-    chocolate = models.BooleanField(blank=True, null=True, verbose_name='chocolate?')
-    other_production = models.CharField(max_length=254, blank=True, null=True,
-                                        verbose_name='Other?')
-    unique_feature_or_activity = RichTextField(blank=True, null=True,
-                                               verbose_name='Uniquely different property feature or activity of note?')
-
-    fridge_nibbles = models.BooleanField(blank=True, null=True, verbose_name='Refrigerated nibbles?')
-    counter_service_casual_fare = models.BooleanField(blank=True, null=True,
-                                                      verbose_name='Counter service casual fare?')
-    table_service_restaurant = models.BooleanField(blank=True, null=True, verbose_name='Table service restaurant?')
-    fine_dining = models.BooleanField(blank=True, null=True, verbose_name='Fine dining?')
-    outside_picnic_food_welcome = models.BooleanField(blank=True, null=True,
-                                                      verbose_name='Outside picnic food welcome?')
-    tasting_room_style = models.CharField(max_length=20, choices=TASTING_ROOM_STYLE, null=True, default=None,
-                                          blank=True)
-    seating_capacity = models.IntegerField(blank=True, null=True, verbose_name='Seating Capacity')
-    reservations_available = models.BooleanField(blank=True, null=True, verbose_name='Reservations available?')
-    walk_in_limit = models.BooleanField(blank=True, null=True, verbose_name='Quantity limit on walk-in party size?')
-    quantity_limit_on_walkin_party_size = models.CharField(max_length=254, blank=True, null=True, verbose_name='Quantity limit on walk-in party size?')
-    dogs_welcome = models.BooleanField(blank=True, null=True, verbose_name='Dogs welcome?')
-    children_welcome = models.BooleanField(blank=True, null=True, verbose_name='Children welcome?')
-    tastingroom_views  = ParentalManyToManyField("goldbook.ViewsFromSeating", blank=True, verbose_name='Views from Tasting Room seating?')
-    tasting_room_views = models.BooleanField(blank=True, null=True, verbose_name='Views from Tasting Room seating?')
-    tasting_room_views_mountains = models.BooleanField(blank=True, null=True, verbose_name='Mountains?')
-    tasting_room_views_vineyard = models.BooleanField(blank=True, null=True, verbose_name='Vineyard?')
-    tasting_room_views_countryside = models.BooleanField(blank=True, null=True, verbose_name='Countryside?')
-    tasting_room_views_urban = models.BooleanField(blank=True, null=True, verbose_name='Urban Views?')
-    fireplace = models.BooleanField(blank=True, null=True, verbose_name='Fireplace present?')
-    fire_tables = models.BooleanField(blank=True, null=True, verbose_name='Firetables available?')
-    outdoor_heating = models.BooleanField(blank=True, null=True, verbose_name='Outdoor heating available?')
-    shade = models.BooleanField(blank=True, null=True,
-                                verbose_name='Is shade abundantly available via umbrellas, porches, pergolas?')
-    lawn = models.BooleanField(blank=True, null=True, verbose_name='Is there a lawn available for picnics and games?')
-    live_music = ParentalManyToManyField("goldbook.Occurrence", blank=True, verbose_name='Live Music?')
-    food_truck = ParentalManyToManyField("goldbook.Occurrence", blank=True, verbose_name='Food Truck Available?', related_name='food_truck')
-    loging = models.BooleanField(blank=True, null=True, verbose_name='Lodging on premise?')
-    souvenirs = models.BooleanField(blank=True, null=True, verbose_name='Souvenir shopping on premise?')
-    festivals = models.BooleanField(blank=True, null=True, verbose_name='Festivals?')
-    festivals_info = models.TextField(blank=True, null=True, verbose_name='Festivals titles and months')
-    dinner_events = models.BooleanField(blank=True, null=True, verbose_name='Dinner events?')
-    dinner_events_info = models.TextField(blank=True, null=True, verbose_name='Dinner event titles & months')
-    classes_or_workshops = models.BooleanField(blank=True, null=True, verbose_name='Classes or workshops?')
-    classes_or_workshops_info = models.TextField(blank=True, null=True,
-                                                 verbose_name='Classes or workshops titles & months')
-    corporate_events = models.BooleanField(blank=True, null=True, verbose_name='Corporate events?')
-    private_party_events = models.BooleanField(blank=True, null=True, verbose_name='Private party events?')
-    minimum_private_party_resv = models.IntegerField(blank=True, null=True,
-                                                     verbose_name='Minimum required for private party reservations')
-    maximum_private_party_resv = models.IntegerField(blank=True, null=True,
-                                                     verbose_name='Maximum required for private party reservations')
-    wedding_events = models.BooleanField(blank=True, null=True, verbose_name='Weddings?')
-    wedding_event_capacity = models.IntegerField(blank=True, null=True, verbose_name='Wedding capacity')
-    wedding_event_avg_per_year = models.IntegerField(blank=True, null=True,
-                                                     verbose_name='Average number of wedding per year')
-    wedding_event_price_range = models.CharField(max_length=254, blank=True, null=True,
-                                                 verbose_name='Average price range of weddings hosted')
-    winery_catering_available = models.BooleanField(blank=True, null=True,
-                                                    verbose_name='Winery provided catering available?')
-    winery_catering_required = models.BooleanField(blank=True, null=True,
-                                                   verbose_name='Winery provided catering Required?')
-    designated_ceremony_site = models.BooleanField(blank=True, null=True, verbose_name='Designated ceremony site?')
-    ceremony_views  = ParentalManyToManyField("goldbook.ViewsFromSeating", blank=True, verbose_name='Views from Ceremony?', related_name='ceremony_views')
-
-    ceremony_views_mountain = models.BooleanField(blank=True, null=True, verbose_name='Ceremony Mountain Views')
-    ceremony_views_vineyard = models.BooleanField(blank=True, null=True, verbose_name='Ceremony Vineyard Views')
-    ceremony_views_countryside = models.BooleanField(blank=True, null=True, verbose_name='Ceremony Countryside Views')
-    ceremony_views_urban = models.BooleanField(blank=True, null=True, verbose_name='Ceremony Urban Views')
-    designated_reception_hall = models.BooleanField(blank=True, null=True, verbose_name='Designated Reception Hall?')
-    designated_reception_hall_views  = ParentalManyToManyField("goldbook.ViewsFromSeating", blank=True, verbose_name='Views from Reception Hall?', related_name='reception_hall_views')
-
-    designated_reception_hall_views_mountain = models.BooleanField(blank=True, null=True,
-                                                                   verbose_name='Designated Reception Hall Mountain Views')
-    designated_reception_hall_views_vineyard = models.BooleanField(blank=True, null=True,
-                                                                   verbose_name='Designated Reception Hall Vineyard Views')
-    designated_reception_hall_views_countryside = models.BooleanField(blank=True, null=True,
-                                                                      verbose_name='Designated Reception Hall Countryside Views')
-    designated_reception_hall_views_urban = models.BooleanField(blank=True, null=True,
-                                                                verbose_name='Designated Reception Hall Urban Views')
-    familiar_with_wc_life = models.BooleanField(blank=True, null=True,
-                                                verbose_name='Are you familiar with Wine & Country Life?')
-    display_wc_life_tasting_room = models.BooleanField(blank=True, null=True,
-                                                       verbose_name='Do you display it in the Tasting Room?')
-    wc_life_advertiser = models.BooleanField(blank=True, null=True,
-                                             verbose_name='Do you currently advertise in WC.Life?')
-    familiar_with_wc_weddings = models.BooleanField(blank=True, null=True,
-                                                    verbose_name='Are you familiar with Wine & Country Weddings?')
-    display_wc_weddings_tasting_room = models.BooleanField(blank=True, null=True,
-                                                           verbose_name='Do you display it in the Tasting Room?')
-    wc_weddings_advertiser = models.BooleanField(blank=True, null=True,
-                                                 verbose_name='Do you currently advertise in WC.Weddings?')
-    familiar_with_wc_goldbook = models.BooleanField(blank=True, null=True,
-                                                    verbose_name='Are you familiar with The Wine & Country Gold Book?')
-    sell_wc_goldbook = models.BooleanField(blank=True, null=True,
-                                           verbose_name='Do they currently sell copies of the Gold Book?')
-    wc_goldbook_advertiser = models.BooleanField(blank=True, null=True,
-                                                 verbose_name='Do they currently advertise in WC.Gold Book?')
-
-    logo = models.ForeignKey(
-        'wagtailimages.Image',
-        null=True,
-        blank=True,
-        on_delete=models.SET_NULL,
-        related_name='winery_logo'
-    )
-    address = StreamField([
-        ('map_struct', blocks.StructBlock([
-            ('address', GeoAddressBlock(required=True)),
-            ('map', GeoBlock(address_field='address')),
-        ]))
-
-    ], blank=True)
-
-    address.verbose_name = 'Main Address'
-
-    tasting_room_address = StreamField([
-        ('map_struct', blocks.StructBlock([
-            ('address', GeoAddressBlock(required=False)),
-            ('map', GeoBlock(address_field='tasting_room_address')),
-        ], ),)
-
-    ], blank=True)
-    tasting_room_address.verbose_name = 'Tasting Room Address (if different)'
-
-    # Search index configuration
-
-    search_fields = Page.search_fields + [
-        index.SearchField('description'),
-    ]
-
-    # Editor panels configuration
-
-    page_content_panels = Page.content_panels
-
-    contact_info_panels = [
-
-        MultiFieldPanel(
-            [
-                FieldRowPanel([
-                    FieldPanel('primary_contact_name'),
-                    FieldPanel('primary_contact_title'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('primary_contact_phone'),
-                    FieldPanel('primary_contact_email'),
-                ]),
-            ],
-            heading="Primary Contact Info",
-        ),
-
-        MultiFieldPanel(
-            [
-                FieldRowPanel([
-                    FieldPanel('secondary_contact_name'),
-                    FieldPanel('secondary_contact_title'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('secondary_contact_phone'),
-                    FieldPanel('secondary_contact_email'),
-                ]),
-            ],
-            heading="Secondary Contact Info",
-        ),
-        MultiFieldPanel(
-            [
-                FieldRowPanel([
-                    FieldPanel('owner_name'),
-                    FieldPanel('owner_phone'),
-                    FieldPanel('owner_email'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('owner_bio'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('winemaker_name'),
-                    FieldPanel('winemaker_phone'),
-                    FieldPanel('winemaker_email'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('winemaker_bio'),
-                ]),
-            ],
-            heading="Owner and Winemaker Info",
-        ),
-
-    ]
-
-    address_panels = [
-        MultiFieldPanel(
-            [
-                FieldPanel('phone_number'),
-                FieldPanel('email'),
-            ],
-            heading="Main Phone and Email Address",
-        ),
-        MultiFieldPanel(
-            [
-                StreamFieldPanel('address'),
-            ],
-            heading="Address",
-        ),
-        MultiFieldPanel(
-            [
-                StreamFieldPanel('tasting_room_address'),
-            ],
-            heading="Tasting Room Address (if different)",
-        ),
-
-    ]
-    media_panels = [
-        MultiFieldPanel(
-            [
-                ImageChooserPanel('logo'),
-            ],
-            heading="Media",
-        ),
-    ]
-
-    description_panels = [
-        FieldPanel('description', classname="full"),
-
-    ]
-
-    winery_panels = [
-        MultiFieldPanel(
-            [
-                FieldRowPanel([
-                    FieldPanel('year_established'),
-                    FieldPanel('number_of_wines'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('total_number_wine_cases_annually'),
-                    FieldPanel('number_of_acres_under_vine'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('ava'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('winery_region'),
-                    FieldPanel('tasting_room_within_vineyard'),
-                ]),
-                # FieldRowPanel([
-                #     FieldPanel('trail_a_part_of', widget=forms.CheckboxSelectMultiple)
-                # ]),
-
-                FieldRowPanel([
-                    FieldPanel('wine_tours_available'),
-                    FieldPanel('wines_sold_online'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('wine_club'),
-                    FieldPanel('num_wine_club_members'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('num_gov_cup_medals'),
-                    FieldPanel('num_other_medals'),
-                ]),
-            ],
-            heading="Winery Info",
-        ),
-    ]
-
-    production_panels = [
-        MultiFieldPanel(
-            [
-                FieldRowPanel([
-                    FieldPanel('brewery'),
-                    FieldPanel('veg_garden'),
-                    FieldPanel('flower_garden'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('bee_apiary'),
-                    FieldPanel('sheep'),
-                    FieldPanel('goats'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('chicken'),
-                    FieldPanel('cattle'),
-                    FieldPanel('horses'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('honey'),
-                    FieldPanel('jelly'),
-                    FieldPanel('cheese'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('chocolate'),
-                    FieldPanel('other_production'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('unique_feature_or_activity'),
-                ]),
-            ],
-            heading="Other Production",
-        ),
-    ]
-
-    food_panels = [
-        MultiFieldPanel(
-            [
-                FieldRowPanel([
-                    FieldPanel('fridge_nibbles'),
-                    FieldPanel('counter_service_casual_fare'),
-                    FieldPanel('table_service_restaurant'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('fine_dining'),
-                    FieldPanel('outside_picnic_food_welcome'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('food_truck', widget=forms.CheckboxSelectMultiple),
-                ]),
-            ],
-            heading="Food",
-        ),
-    ]
-
-    tasting_room_panels = [
-        MultiFieldPanel(
-            [
-                FieldRowPanel([
-                    FieldPanel('tasting_room_style'),
-                    FieldPanel('seating_capacity'),
-                    FieldPanel('reservations_available'),
-
-                ]),
-                FieldRowPanel([
-                    FieldPanel('quantity_limit_on_walkin_party_size'),
-                    FieldPanel('dogs_welcome'),
-                    FieldPanel('children_welcome'),
-
-                ]),
-                FieldRowPanel([
-                    FieldPanel('tastingroom_views', widget=forms.CheckboxSelectMultiple),
-
-                ]),
-
-                FieldRowPanel([
-                    FieldPanel('fireplace'),
-                    FieldPanel('fire_tables'),
-                    FieldPanel('outdoor_heating'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('shade'),
-                    FieldPanel('lawn'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel("live_music", widget=forms.CheckboxSelectMultiple)
-                ]),
-                FieldRowPanel([
-                    FieldPanel('loging'),
-                    FieldPanel('souvenirs'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('festivals'),
-                    FieldPanel('festivals_info'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('dinner_events'),
-                    FieldPanel('dinner_events_info'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('classes_or_workshops'),
-                    FieldPanel('classes_or_workshops_info'),
-                ]),
-            ],
-            heading="Tasting Room Experience",
-        ),
-    ]
-
-    event_services_panels = [
-        MultiFieldPanel(
-            [
-                FieldRowPanel([
-                    FieldPanel('corporate_events'),
-                    FieldPanel('private_party_events'),
-
-                ]),
-                FieldRowPanel([
-                    FieldPanel('minimum_private_party_resv'),
-                    FieldPanel('maximum_private_party_resv'),
-
-                ]),
-                FieldRowPanel([
-                    FieldPanel('wedding_events'),
-                    FieldPanel('wedding_event_capacity'),
-
-                ]),
-                FieldRowPanel([
-                    FieldPanel('wedding_event_avg_per_year'),
-                    FieldPanel('wedding_event_price_range'),
-
-                ]),
-                FieldRowPanel([
-                    FieldPanel('winery_catering_available'),
-                    FieldPanel('winery_catering_required'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('designated_ceremony_site'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('ceremony_views', widget=forms.CheckboxSelectMultiple),
-
-                ]),
-
-                FieldRowPanel([
-                    FieldPanel('designated_reception_hall'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('designated_reception_hall_views', widget=forms.CheckboxSelectMultiple),
-
-                ]),
-
-            ],
-            heading="Event Services",
-        ),
-    ]
-
-    advertising_info_panels = [
-        MultiFieldPanel(
-            [
-                FieldRowPanel([
-                    FieldPanel('familiar_with_wc_life'),
-                    FieldPanel('display_wc_life_tasting_room'),
-                    FieldPanel('wc_life_advertiser'),
-
-                ]),
-                FieldRowPanel([
-                    FieldPanel('familiar_with_wc_weddings'),
-                    FieldPanel('display_wc_weddings_tasting_room'),
-                    FieldPanel('wc_weddings_advertiser'),
-                ]),
-                FieldRowPanel([
-                    FieldPanel('familiar_with_wc_goldbook'),
-                    FieldPanel('sell_wc_goldbook'),
-                    FieldPanel('wc_goldbook_advertiser'),
-                ]),
-            ],
-            heading="Advertising Info",
-        ),
-    ]
-
-    notes_panels = [
-        MultiFieldPanel(
-            [
-                FieldPanel('notes'),
-            ],
-            heading="Notes",
-        ),
-    ]
-
-    combined_info_panels = Page.content_panels + \
-                           contact_info_panels + \
-                           address_panels + \
-                           winery_panels + \
-                           production_panels + \
-                           food_panels + \
-                           tasting_room_panels + \
-                           event_services_panels + \
-                           advertising_info_panels
-
-    edit_handler = TabbedInterface(
-        [
-            ObjectList(combined_info_panels, heading='Information/Questionaire'),
-            # This is our custom banner_panels. It's just a list, how easy!
-            # ObjectList(page_content_panels, heading="Basic Info"),
-            # ObjectList(contact_info_panels, heading="Contact Info"),
-            # ObjectList(address_panels, heading="Address/Phone/Email"),
-            # ObjectList(winery_panels, heading="Winery Info"),
-            # ObjectList(production_panels, heading="Other Production"),
-            # ObjectList(food_panels, heading="Food"),
-            # ObjectList(tasting_room_panels, heading="Tasting Room Experience"),
-            # ObjectList(event_services_panels, heading="Event Services"),
-            # ObjectList(advertising_info_panels, heading="Advertising Info"),
-            # ObjectList(media_panels, heading="Media"),
-            # ObjectList(notes_panels, heading="Notes"),
-            # ObjectList(Page.promote_panels, heading='Promotional Stuff'),
-            # ObjectList(Page.settings_panels, heading='Settings Stuff'),
-        ]
-    )
-
-
-Winery._meta.get_field("title").verbose_name = "Winery Name"
+from django import forms
+from django.db import models
+from django.utils.translation import gettext_lazy as _
+from modelcluster.fields import ParentalManyToManyField
+from phonenumber_field.modelfields import PhoneNumberField
+from wagtail import blocks
+from wagtail.admin.panels import (
+    FieldPanel,
+    MultiFieldPanel,
+    FieldRowPanel,
+    ObjectList,
+    TabbedInterface,
+)
+from wagtail.fields import StreamField, RichTextField
+from wagtail.models import Page, Orderable
+from wagtail.search import index
+from wagtail.snippets.models import register_snippet
+from wagtailgeowidget.blocks import GeoBlock, GeoAddressBlock
+
+from goldbook.choices import TASTING_ROOM_STYLE
+from goldbook.util.helpers import my_year_validator
+
+
+@register_snippet
+class Occurrence(Orderable):
+    name = models.CharField(
+        verbose_name=_('Name'),
+        max_length=255,
+        help_text=_("The name of the Occurrence as you'd like it to be seen by the public")
+    )
+    slug = models.SlugField(
+        verbose_name=_('slug'),
+        allow_unicode=True,
+        max_length=255,
+        help_text=_("The name of the region as it will appear in URLs e.g http://domain.com/wineries/northern-va/")
+    )
+
+    class Meta:
+        verbose_name = 'Occurrence'
+        verbose_name_plural = 'Occurrences'
+
+    def __str__(self):
+        return self.name
+
+    panels = [
+        FieldPanel('name'),
+        FieldPanel('slug'),
+    ]
+
+
+@register_snippet
+class WineTrail(Orderable):
+    name = models.CharField(
+        verbose_name=_('Name'),
+        max_length=255,
+        help_text=_("The name of the Wine Trail as you'd like it to be seen by the public")
+    )
+    slug = models.SlugField(
+        verbose_name=_('slug'),
+        allow_unicode=True,
+        max_length=255,
+        help_text=_("The name of the Wine Trail  as it will appear in URLs e.g http://domain.com/wineries/pub-crawl/")
+    )
+
+    class Meta:
+        verbose_name = 'Wine Trail'
+        verbose_name_plural = 'Wine Trails'
+
+    def __str__(self):
+        return self.name
+
+    panels = [
+        FieldPanel('name'),
+        FieldPanel('slug'),
+    ]
+
+
+@register_snippet
+class AVA(Orderable):
+    name = models.CharField(
+        verbose_name=_('Name'),
+        max_length=255,
+        help_text=_("The name of the AVA as you'd like it to be seen by the public")
+    )
+    slug = models.SlugField(
+        verbose_name=_('slug'),
+        allow_unicode=True,
+        max_length=255,
+        help_text=_("The name of the AVA  as it will appear in URLs e.g http://domain.com/wineries/ava/blue-ridge/")
+    )
+
+    class Meta:
+        verbose_name = 'AVA'
+        verbose_name_plural = 'AVAs'
+
+    def __str__(self):
+        return self.name
+
+    panels = [
+        FieldPanel('name'),
+        FieldPanel('slug'),
+    ]
+
+
+# class OperatingHours(models.Model):
+#     """
+#     A Django model to capture operating hours for a Location
+#     """
+#
+#     day = models.CharField(
+#         max_length=4,
+#         choices=DAY_CHOICES,
+#         default='MON'
+#     )
+#     opening_time = models.TimeField(
+#         blank=True,
+#         null=True
+#     )
+#     closing_time = models.TimeField(
+#         blank=True,
+#         null=True
+#     )
+#     closed = models.BooleanField(
+#         "Closed?",
+#         blank=True,
+#         help_text='Tick if location is closed on this day'
+#     )
+#
+#     panels = [
+#         FieldPanel('day'),
+#         FieldPanel('opening_time'),
+#         FieldPanel('closing_time'),
+#         FieldPanel('closed'),
+#     ]
+#
+#     class Meta:
+#         abstract = True
+#
+#     def __str__(self):
+#         if self.opening_time:
+#             opening = self.opening_time.strftime('%H:%M')
+#         else:
+#             opening = '--'
+#         if self.closing_time:
+#             closed = self.closing_time.strftime('%H:%M')
+#         else:
+#             closed = '--'
+#         return '{}: {} - {} {}'.format(
+#             self.day,
+#             opening,
+#             closed,
+#             settings.TIME_ZONE
+#         )
+#
+#
+# class WineryOperatingHours(Orderable, OperatingHours):
+#     """
+#     A model creating a relationship between the OperatingHours and Location
+#     Note that unlike BlogPeopleRelationship we don't include a ForeignKey to
+#     OperatingHours as we don't need that relationship (e.g. any Location open
+#     a certain day of the week). The ParentalKey is the minimum required to
+#     relate the two objects to one another. We use the ParentalKey's related_
+#     name to access it from the LocationPage admin
+#     """
+#     location = ParentalKey(
+#         'WineryOld',
+#         related_name='hours_of_operation',
+#         on_delete=models.CASCADE
+#     )
+
+@register_snippet
+class WineryRegion(Orderable):
+    name = models.CharField(
+        verbose_name=_('Name'),
+        max_length=255,
+        help_text=_("The name of the Region as you'd like it to be seen by the public")
+    )
+    slug = models.SlugField(
+        verbose_name=_('slug'),
+        allow_unicode=True,
+        max_length=255,
+        help_text=_("The name of the region as it will appear in URLs e.g http://domain.com/wineries/northern-va/")
+    )
+
+    class Meta:
+        verbose_name = 'Winery Region'
+        verbose_name_plural = 'Winery Regions'
+
+    def __str__(self):
+        return self.name
+
+    panels = [
+        FieldPanel('name'),
+        FieldPanel('slug'),
+    ]
+
+
+@register_snippet
+class ViewsFromSeating(Orderable):
+    name = models.CharField(
+        verbose_name=_('Name'),
+        max_length=255,
+        help_text=_("The name of the View as you'd like it to be seen by the public")
+    )
+    slug = models.SlugField(
+        verbose_name=_('slug'),
+        allow_unicode=True,
+        max_length=255,
+        help_text=_(
+            "The name of the view as it will appear in URLs e.g http://domain.com/wineries/northern-va/lakeviews/")
+    )
+
+    class Meta:
+        verbose_name = 'View From Seating'
+        verbose_name_plural = 'Seating Views'
+
+    def __str__(self):
+        return self.name
+
+    panels = [
+        FieldPanel('name'),
+        FieldPanel('slug'),
+    ]
+
+
+class WineriesIndexPage(Page):
+    template = 'goldbook/wineries_page.html'
+    max_count = 1
+    subpage_types = [
+        'goldbook.Winery',  # appname.ModelName
+    ]
+
+    class Meta:
+        verbose_name_plural = 'Wineries'
+        verbose_name = 'Wineries'
+
+
+class Winery(Page):
+    subpage_types = []
+    description = RichTextField(null=True, blank=True)
+    notes = RichTextField(null=True, blank=True)
+    phone_number = PhoneNumberField(blank=True, null=True, verbose_name='Business Phone')
+    email = models.EmailField(max_length=254, blank=True, null=True, verbose_name='Business Email')
+    year_established = models.IntegerField(validators=[my_year_validator], blank=True, null=True,
+                                           verbose_name='Year established')
+    number_of_wines = models.IntegerField(blank=True, null=True, verbose_name='Number of Wines Produced')
+    total_number_wine_cases_annually = models.IntegerField(blank=True, null=True,
+                                                           verbose_name='Total number of cases in production annually')
+    number_of_acres_under_vine = models.IntegerField(blank=True, null=True, verbose_name='Number of acres under vine')
+    winery_region = models.ForeignKey('goldbook.WineryRegion', null=True, blank=True, on_delete=models.SET_NULL,
+                                      verbose_name='Region of VA', related_name='+')
+    ava = models.ForeignKey('goldbook.AVA', blank=True, null=True, on_delete=models.SET_NULL,
+                            verbose_name='AVA', related_name='+')
+    trail_a_part_of = ParentalManyToManyField("goldbook.WineTrail", blank=True, verbose_name='Trail a part of')
+    largest_town_within_30_mins = models.CharField(max_length=254, blank=True, null=True,
+                                                   verbose_name='Largest town within 30 min')
+    tasting_room_within_vineyard = models.BooleanField(blank=True, null=True,
+                                                       verbose_name='Is the Tasting Room located within a vineyard?')
+    wine_tours_available = models.BooleanField(blank=True, null=True, verbose_name='Winery tours available?')
+    wines_sold_online = models.BooleanField(blank=True, null=True, verbose_name='Wines sold online?')
+    wine_club = models.BooleanField(blank=True, null=True, verbose_name='Wines Club?')
+    num_wine_club_members = models.IntegerField(blank=True, null=True, verbose_name='Number of Wine Club members?')
+    num_gov_cup_medals = models.IntegerField(blank=True, null=True,
+                                             verbose_name='Number of Gov Cup Gold medals over the years?')
+    num_other_medals = models.IntegerField(blank=True, null=True, verbose_name='Number of other gold medals of note')
+
+    primary_contact_name = models.CharField(max_length=254, blank=True, null=True, verbose_name='Primary Contact Name')
+    primary_contact_title = models.CharField(max_length=254, blank=True, null=True,
+                                             verbose_name='Primary Contact Title')
+    primary_contact_phone = models.CharField(max_length=254, blank=True, null=True,
+                                             verbose_name='Primary Contact Phone')
+    primary_contact_email = models.CharField(max_length=254, blank=True, null=True,
+                                             verbose_name='Primary Contact email')
+    secondary_contact_name = models.CharField(max_length=254, blank=True, null=True,
+                                              verbose_name='Secondary Contact Name')
+    secondary_contact_title = models.CharField(max_length=254, blank=True, null=True,
+                                               verbose_name='Secondary Contact Title')
+    secondary_contact_phone = models.CharField(max_length=254, blank=True, null=True,
+                                               verbose_name='Secondary Contact Phone')
+    secondary_contact_email = models.CharField(max_length=254, blank=True, null=True,
+                                               verbose_name='Secondary Contact email')
+    owner_name = models.CharField(max_length=254, blank=True, null=True,
+                                  verbose_name='Owner Name')
+    owner_phone = models.CharField(max_length=254, blank=True, null=True,
+                                   verbose_name='Owner Phone')
+    owner_email = models.CharField(max_length=254, blank=True, null=True,
+                                   verbose_name='Owner email')
+    owner_bio = RichTextField(null=True, blank=True, verbose_name='Owner Bio')
+    winemaker_name = models.CharField(max_length=254, blank=True, null=True,
+                                      verbose_name='Winemaker Name')
+    winemaker_phone = models.CharField(max_length=254, blank=True, null=True,
+                                       verbose_name='Winemaker Phone')
+    winemaker_email = models.CharField(max_length=254, blank=True, null=True,
+                                       verbose_name='Winemaker email')
+    winemaker_bio = RichTextField(null=True, blank=True, verbose_name='Winemaker Bio')
+    brewery = models.BooleanField(blank=True, null=True, verbose_name='Brewery?')
+    veg_garden = models.BooleanField(blank=True, null=True, verbose_name='Vegetable or fruit garden on premise?')
+    flower_garden = models.BooleanField(blank=True, null=True, verbose_name='Formal or flower garden on premise?')
+    bee_apiary = models.BooleanField(blank=True, null=True, verbose_name='Bee apiary on premise?')
+    sheep = models.BooleanField(blank=True, null=True, verbose_name='Sheep on premise?')
+    goats = models.BooleanField(blank=True, null=True, verbose_name='Goats on premise?')
+    chicken = models.BooleanField(blank=True, null=True, verbose_name='Chickens on premise?')
+    cattle = models.BooleanField(blank=True, null=True, verbose_name='Cattle on premise?')
+    horses = models.BooleanField(blank=True, null=True, verbose_name='Horses on premise?')
+    honey = models.BooleanField(blank=True, null=True, verbose_name='honey?')
+    jelly = models.BooleanField(blank=True, null=True, verbose_name='jelly?')
+    cheese = models.BooleanField(blank=True, null=True, verbose_name='cheese?')
+    chocolate = models.BooleanField(blank=True, null=True, verbose_name='chocolate?')
+    other_production = models.CharField(max_length=254, blank=True, null=True,
+                                        verbose_name='Other?')
+    unique_feature_or_activity = RichTextField(blank=True, null=True,
+                                               verbose_name='Uniquely different property feature or activity of note?')
+
+    fridge_nibbles = models.BooleanField(blank=True, null=True, verbose_name='Refrigerated nibbles?')
+    counter_service_casual_fare = models.BooleanField(blank=True, null=True,
+                                                      verbose_name='Counter service casual fare?')
+    table_service_restaurant = models.BooleanField(blank=True, null=True, verbose_name='Table service restaurant?')
+    fine_dining = models.BooleanField(blank=True, null=True, verbose_name='Fine dining?')
+    outside_picnic_food_welcome = models.BooleanField(blank=True, null=True,
+                                                      verbose_name='Outside picnic food welcome?')
+    tasting_room_style = models.CharField(max_length=20, choices=TASTING_ROOM_STYLE, null=True, default=None,
+                                          blank=True)
+    seating_capacity = models.IntegerField(blank=True, null=True, verbose_name='Seating Capacity')
+    reservations_available = models.BooleanField(blank=True, null=True, verbose_name='Reservations available?')
+    walk_in_limit = models.BooleanField(blank=True, null=True, verbose_name='Quantity limit on walk-in party size?')
+    quantity_limit_on_walkin_party_size = models.CharField(max_length=254, blank=True, null=True,
+                                                           verbose_name='Quantity limit on walk-in party size?')
+    dogs_welcome = models.BooleanField(blank=True, null=True, verbose_name='Dogs welcome?')
+    children_welcome = models.BooleanField(blank=True, null=True, verbose_name='Children welcome?')
+    tastingroom_views = ParentalManyToManyField("goldbook.ViewsFromSeating", blank=True,
+                                                verbose_name='Views from Tasting Room seating?')
+    tasting_room_views = models.BooleanField(blank=True, null=True, verbose_name='Views from Tasting Room seating?')
+    tasting_room_views_mountains = models.BooleanField(blank=True, null=True, verbose_name='Mountains?')
+    tasting_room_views_vineyard = models.BooleanField(blank=True, null=True, verbose_name='Vineyard?')
+    tasting_room_views_countryside = models.BooleanField(blank=True, null=True, verbose_name='Countryside?')
+    tasting_room_views_urban = models.BooleanField(blank=True, null=True, verbose_name='Urban Views?')
+    fireplace = models.BooleanField(blank=True, null=True, verbose_name='Fireplace present?')
+    fire_tables = models.BooleanField(blank=True, null=True, verbose_name='Firetables available?')
+    outdoor_heating = models.BooleanField(blank=True, null=True, verbose_name='Outdoor heating available?')
+    shade = models.BooleanField(blank=True, null=True,
+                                verbose_name='Is shade abundantly available via umbrellas, porches, pergolas?')
+    lawn = models.BooleanField(blank=True, null=True, verbose_name='Is there a lawn available for picnics and games?')
+    live_music = ParentalManyToManyField("goldbook.Occurrence", blank=True, verbose_name='Live Music?')
+    food_truck = ParentalManyToManyField("goldbook.Occurrence", blank=True, verbose_name='Food Truck Available?',
+                                         related_name='food_truck')
+    loging = models.BooleanField(blank=True, null=True, verbose_name='Lodging on premise?')
+    souvenirs = models.BooleanField(blank=True, null=True, verbose_name='Souvenir shopping on premise?')
+    festivals = models.BooleanField(blank=True, null=True, verbose_name='Festivals?')
+    festivals_info = models.TextField(blank=True, null=True, verbose_name='Festivals titles and months')
+    dinner_events = models.BooleanField(blank=True, null=True, verbose_name='Dinner events?')
+    dinner_events_info = models.TextField(blank=True, null=True, verbose_name='Dinner event titles & months')
+    classes_or_workshops = models.BooleanField(blank=True, null=True, verbose_name='Classes or workshops?')
+    classes_or_workshops_info = models.TextField(blank=True, null=True,
+                                                 verbose_name='Classes or workshops titles & months')
+    corporate_events = models.BooleanField(blank=True, null=True, verbose_name='Corporate events?')
+    private_party_events = models.BooleanField(blank=True, null=True, verbose_name='Private party events?')
+    minimum_private_party_resv = models.IntegerField(blank=True, null=True,
+                                                     verbose_name='Minimum required for private party reservations')
+    maximum_private_party_resv = models.IntegerField(blank=True, null=True,
+                                                     verbose_name='Maximum required for private party reservations')
+    wedding_events = models.BooleanField(blank=True, null=True, verbose_name='Weddings?')
+    wedding_event_capacity = models.IntegerField(blank=True, null=True, verbose_name='Wedding capacity')
+    wedding_event_avg_per_year = models.IntegerField(blank=True, null=True,
+                                                     verbose_name='Average number of wedding per year')
+    wedding_event_price_range = models.CharField(max_length=254, blank=True, null=True,
+                                                 verbose_name='Average price range of weddings hosted')
+    winery_catering_available = models.BooleanField(blank=True, null=True,
+                                                    verbose_name='Winery provided catering available?')
+    winery_catering_required = models.BooleanField(blank=True, null=True,
+                                                   verbose_name='Winery provided catering Required?')
+    designated_ceremony_site = models.BooleanField(blank=True, null=True, verbose_name='Designated ceremony site?')
+    ceremony_views = ParentalManyToManyField("goldbook.ViewsFromSeating", blank=True,
+                                             verbose_name='Views from Ceremony?', related_name='ceremony_views')
+
+    ceremony_views_mountain = models.BooleanField(blank=True, null=True, verbose_name='Ceremony Mountain Views')
+    ceremony_views_vineyard = models.BooleanField(blank=True, null=True, verbose_name='Ceremony Vineyard Views')
+    ceremony_views_countryside = models.BooleanField(blank=True, null=True, verbose_name='Ceremony Countryside Views')
+    ceremony_views_urban = models.BooleanField(blank=True, null=True, verbose_name='Ceremony Urban Views')
+    designated_reception_hall = models.BooleanField(blank=True, null=True, verbose_name='Designated Reception Hall?')
+    designated_reception_hall_views = ParentalManyToManyField("goldbook.ViewsFromSeating", blank=True,
+                                                              verbose_name='Views from Reception Hall?',
+                                                              related_name='reception_hall_views')
+
+    designated_reception_hall_views_mountain = models.BooleanField(blank=True, null=True,
+                                                                   verbose_name='Designated Reception Hall Mountain Views')
+    designated_reception_hall_views_vineyard = models.BooleanField(blank=True, null=True,
+                                                                   verbose_name='Designated Reception Hall Vineyard Views')
+    designated_reception_hall_views_countryside = models.BooleanField(blank=True, null=True,
+                                                                      verbose_name='Designated Reception Hall Countryside Views')
+    designated_reception_hall_views_urban = models.BooleanField(blank=True, null=True,
+                                                                verbose_name='Designated Reception Hall Urban Views')
+    familiar_with_wc_life = models.BooleanField(blank=True, null=True,
+                                                verbose_name='Are you familiar with Wine & Country Life?')
+    display_wc_life_tasting_room = models.BooleanField(blank=True, null=True,
+                                                       verbose_name='Do you display it in the Tasting Room?')
+    wc_life_advertiser = models.BooleanField(blank=True, null=True,
+                                             verbose_name='Do you currently advertise in WC.Life?')
+    familiar_with_wc_weddings = models.BooleanField(blank=True, null=True,
+                                                    verbose_name='Are you familiar with Wine & Country Weddings?')
+    display_wc_weddings_tasting_room = models.BooleanField(blank=True, null=True,
+                                                           verbose_name='Do you display it in the Tasting Room?')
+    wc_weddings_advertiser = models.BooleanField(blank=True, null=True,
+                                                 verbose_name='Do you currently advertise in WC.Weddings?')
+    familiar_with_wc_goldbook = models.BooleanField(blank=True, null=True,
+                                                    verbose_name='Are you familiar with The Wine & Country Gold Book?')
+    sell_wc_goldbook = models.BooleanField(blank=True, null=True,
+                                           verbose_name='Do they currently sell copies of the Gold Book?')
+    wc_goldbook_advertiser = models.BooleanField(blank=True, null=True,
+                                                 verbose_name='Do they currently advertise in WC.Gold Book?')
+
+    logo = models.ForeignKey(
+        'wagtailimages.Image',
+        null=True,
+        blank=True,
+        on_delete=models.SET_NULL,
+        related_name='winery_logo'
+    )
+    address = StreamField([
+        ('map_struct', blocks.StructBlock([
+            ('address', GeoAddressBlock(required=True)),
+            ('map', GeoBlock(address_field='address')),
+        ]))
+
+    ], blank=True, use_json_field=True)
+
+    address.verbose_name = 'Main Address'
+
+    tasting_room_address = StreamField([
+        ('map_struct', blocks.StructBlock([
+            ('address', GeoAddressBlock(required=False)),
+            ('map', GeoBlock(address_field='tasting_room_address')),
+        ], ),)
+
+    ], blank=True, use_json_field=True)
+    tasting_room_address.verbose_name = 'Tasting Room Address (if different)'
+
+    # Search index configuration
+
+    search_fields = Page.search_fields + [
+        index.SearchField('description'),
+    ]
+
+    # Editor panels configuration
+
+    page_content_panels = [MultiFieldPanel(
+        [
+            FieldPanel('title'),
+        ],
+        heading="Winery Name",
+    ),
+    ]
+
+    contact_info_panels = [
+        MultiFieldPanel(
+            [
+                FieldPanel('title'),
+            ],
+            heading="Winery Name",
+        ),
+
+        MultiFieldPanel(
+            [
+                FieldRowPanel([
+                    FieldPanel('primary_contact_name'),
+                    FieldPanel('primary_contact_title'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('primary_contact_phone'),
+                    FieldPanel('primary_contact_email'),
+                ]),
+            ],
+            heading="Primary Contact Info",
+        ),
+
+        MultiFieldPanel(
+            [
+                FieldRowPanel([
+                    FieldPanel('secondary_contact_name'),
+                    FieldPanel('secondary_contact_title'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('secondary_contact_phone'),
+                    FieldPanel('secondary_contact_email'),
+                ]),
+            ],
+            heading="Secondary Contact Info",
+        ),
+        MultiFieldPanel(
+            [
+                FieldRowPanel([
+                    FieldPanel('owner_name'),
+                    FieldPanel('owner_phone'),
+                    FieldPanel('owner_email'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('owner_bio'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('winemaker_name'),
+                    FieldPanel('winemaker_phone'),
+                    FieldPanel('winemaker_email'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('winemaker_bio'),
+                ]),
+            ],
+            heading="Owner and Winemaker Info",
+        ),
+
+    ]
+
+    address_panels = [
+        MultiFieldPanel(
+            [
+                FieldPanel('phone_number'),
+                FieldPanel('email'),
+            ],
+            heading="Main Phone and Email Address",
+        ),
+        MultiFieldPanel(
+            [
+                FieldPanel('address'),
+            ],
+            heading="Address",
+        ),
+        MultiFieldPanel(
+            [
+                FieldPanel('tasting_room_address'),
+            ],
+            heading="Tasting Room Address (if different)",
+        ),
+
+    ]
+    media_panels = [
+        MultiFieldPanel(
+            [
+                FieldPanel('logo'),
+            ],
+            heading="Media",
+        ),
+    ]
+
+    description_panels = [
+        FieldPanel('description', classname="full"),
+
+    ]
+
+    winery_panels = [
+        MultiFieldPanel(
+            [
+                FieldRowPanel([
+                    FieldPanel('year_established'),
+                    FieldPanel('number_of_wines'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('total_number_wine_cases_annually'),
+                    FieldPanel('number_of_acres_under_vine'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('ava'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('winery_region'),
+                    FieldPanel('tasting_room_within_vineyard'),
+                ]),
+                # FieldRowPanel([
+                #     FieldPanel('trail_a_part_of', widget=forms.CheckboxSelectMultiple)
+                # ]),
+
+                FieldRowPanel([
+                    FieldPanel('wine_tours_available'),
+                    FieldPanel('wines_sold_online'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('wine_club'),
+                    FieldPanel('num_wine_club_members'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('num_gov_cup_medals'),
+                    FieldPanel('num_other_medals'),
+                ]),
+            ],
+            heading="Winery Info",
+        ),
+    ]
+
+    production_panels = [
+        MultiFieldPanel(
+            [
+                FieldRowPanel([
+                    FieldPanel('brewery'),
+                    FieldPanel('veg_garden'),
+                    FieldPanel('flower_garden'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('bee_apiary'),
+                    FieldPanel('sheep'),
+                    FieldPanel('goats'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('chicken'),
+                    FieldPanel('cattle'),
+                    FieldPanel('horses'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('honey'),
+                    FieldPanel('jelly'),
+                    FieldPanel('cheese'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('chocolate'),
+                    FieldPanel('other_production'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('unique_feature_or_activity'),
+                ]),
+            ],
+            heading="Other Production",
+        ),
+    ]
+
+    food_panels = [
+        MultiFieldPanel(
+            [
+                FieldRowPanel([
+                    FieldPanel('fridge_nibbles'),
+                    FieldPanel('counter_service_casual_fare'),
+                    FieldPanel('table_service_restaurant'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('fine_dining'),
+                    FieldPanel('outside_picnic_food_welcome'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('food_truck', widget=forms.CheckboxSelectMultiple),
+                ]),
+            ],
+            heading="Food",
+        ),
+    ]
+
+    tasting_room_panels = [
+        MultiFieldPanel(
+            [
+                FieldRowPanel([
+                    FieldPanel('tasting_room_style'),
+                    FieldPanel('seating_capacity'),
+                    FieldPanel('reservations_available'),
+
+                ]),
+                FieldRowPanel([
+                    FieldPanel('quantity_limit_on_walkin_party_size'),
+                    FieldPanel('dogs_welcome'),
+                    FieldPanel('children_welcome'),
+
+                ]),
+                FieldRowPanel([
+                    FieldPanel('tastingroom_views', widget=forms.CheckboxSelectMultiple),
+
+                ]),
+
+                FieldRowPanel([
+                    FieldPanel('fireplace'),
+                    FieldPanel('fire_tables'),
+                    FieldPanel('outdoor_heating'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('shade'),
+                    FieldPanel('lawn'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel("live_music", widget=forms.CheckboxSelectMultiple)
+                ]),
+                FieldRowPanel([
+                    FieldPanel('loging'),
+                    FieldPanel('souvenirs'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('festivals'),
+                    FieldPanel('festivals_info'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('dinner_events'),
+                    FieldPanel('dinner_events_info'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('classes_or_workshops'),
+                    FieldPanel('classes_or_workshops_info'),
+                ]),
+            ],
+            heading="Tasting Room Experience",
+        ),
+    ]
+
+    event_services_panels = [
+        MultiFieldPanel(
+            [
+                FieldRowPanel([
+                    FieldPanel('corporate_events'),
+                    FieldPanel('private_party_events'),
+
+                ]),
+                FieldRowPanel([
+                    FieldPanel('minimum_private_party_resv'),
+                    FieldPanel('maximum_private_party_resv'),
+
+                ]),
+                FieldRowPanel([
+                    FieldPanel('wedding_events'),
+                    FieldPanel('wedding_event_capacity'),
+
+                ]),
+                FieldRowPanel([
+                    FieldPanel('wedding_event_avg_per_year'),
+                    FieldPanel('wedding_event_price_range'),
+
+                ]),
+                FieldRowPanel([
+                    FieldPanel('winery_catering_available'),
+                    FieldPanel('winery_catering_required'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('designated_ceremony_site'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('ceremony_views', widget=forms.CheckboxSelectMultiple),
+
+                ]),
+
+                FieldRowPanel([
+                    FieldPanel('designated_reception_hall'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('designated_reception_hall_views', widget=forms.CheckboxSelectMultiple),
+
+                ]),
+
+            ],
+            heading="Event Services",
+        ),
+    ]
+
+    advertising_info_panels = [
+        MultiFieldPanel(
+            [
+                FieldRowPanel([
+                    FieldPanel('familiar_with_wc_life'),
+                    FieldPanel('display_wc_life_tasting_room'),
+                    FieldPanel('wc_life_advertiser'),
+
+                ]),
+                FieldRowPanel([
+                    FieldPanel('familiar_with_wc_weddings'),
+                    FieldPanel('display_wc_weddings_tasting_room'),
+                    FieldPanel('wc_weddings_advertiser'),
+                ]),
+                FieldRowPanel([
+                    FieldPanel('familiar_with_wc_goldbook'),
+                    FieldPanel('sell_wc_goldbook'),
+                    FieldPanel('wc_goldbook_advertiser'),
+                ]),
+            ],
+            heading="Advertising Info",
+        ),
+    ]
+
+    notes_panels = [
+        MultiFieldPanel(
+            [
+                FieldPanel('notes'),
+            ],
+            heading="Notes",
+        ),
+    ]
+
+    combined_info_panels = Page.content_panels + \
+                           contact_info_panels + \
+                           address_panels + \
+                           winery_panels + \
+                           production_panels + \
+                           food_panels + \
+                           tasting_room_panels + \
+                           event_services_panels + \
+                           advertising_info_panels
+
+    edit_handler = TabbedInterface(
+        [
+            # ObjectList(combined_info_panels, heading='Information/Questionaire'),
+            # This is our custom banner_panels. It's just a list, how easy!
+            # ObjectList(page_content_panels, heading="Basic Info"),
+            ObjectList(contact_info_panels, heading="Basic Info/Contacts"),
+            ObjectList(address_panels, heading="Address/Phone/Email"),
+            ObjectList(winery_panels, heading="Winery Info"),
+            ObjectList(production_panels, heading="Other Production"),
+            ObjectList(food_panels, heading="Food"),
+            ObjectList(tasting_room_panels, heading="Tasting Room Experience"),
+            ObjectList(event_services_panels, heading="Event Services"),
+            ObjectList(advertising_info_panels, heading="Advertising Info"),
+            # ObjectList(media_panels, heading="Media"),
+            # ObjectList(notes_panels, heading="Notes"),
+            # ObjectList(Page.promote_panels, heading='Promotional Stuff'),
+            # ObjectList(Page.settings_panels, heading='Settings Stuff'),
+        ]
+    )
+
+
+Winery._meta.get_field("title").verbose_name = "Winery Name"
```

### Comparing `goldbook-0.1/goldbook/wagtail_hooks.py` & `goldbook-0.2/goldbook/wagtail_hooks.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from wagtail.contrib.modeladmin.options import (
-    ModelAdmin, modeladmin_register)
-from wagtail.core import hooks
-from wagtail.admin.widgets import Button, PageListingButton
-
-@hooks.register('construct_page_listing_buttons')
-def replace_page_listing_button_item(buttons, page, page_perms, is_parent=False, context=None):
-    for index, button in enumerate(buttons):
-       # basic code only - recommend you find a more robust way to confirm this is the add child page button
-        if button.label == 'Add child page':
-            button.label = 'Add New Winery'
-            buttons[index] = button # update the matched button with a new one (note. PageListingButton is used in page listing)
+from wagtail.contrib.modeladmin.options import (
+    ModelAdmin, modeladmin_register)
+from wagtail import hooks
+from wagtail.admin.widgets import Button, PageListingButton
+
+@hooks.register('construct_page_listing_buttons')
+def replace_page_listing_button_item(buttons, page, page_perms, is_parent=False, context=None):
+    for index, button in enumerate(buttons):
+       # basic code only - recommend you find a more robust way to confirm this is the add child page button
+        if button.label == 'Add child page':
+            button.label = 'Add New Winery'
+            buttons[index] = button # update the matched button with a new one (note. PageListingButton is used in page listing)
```

### Comparing `goldbook-0.1/goldbook.egg-info/SOURCES.txt` & `goldbook-0.2/goldbook.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,10 +16,11 @@
 goldbook/migrations/0001_initial.py
 goldbook/migrations/0002_winetrail_remove_winery_trail_a_part_of_and_more.py
 goldbook/migrations/0003_ava_alter_winery_ava.py
 goldbook/migrations/0004_winery_food_truck.py
 goldbook/migrations/0005_winery_quantity_limit_on_walkin_party_size.py
 goldbook/migrations/0006_viewsfromseating_winery_tastingroom_views.py
 goldbook/migrations/0007_winery_ceremony_views_and_more.py
+goldbook/migrations/0008_alter_winery_address_and_more.py
 goldbook/migrations/__init__.py
 goldbook/util/__init__.py
 goldbook/util/helpers.py
```

