# Comparing `tmp/bring-order-0.2.0.tar.gz` & `tmp/bring_order-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bring-order-0.2.0.tar", last modified: Mon Jun 19 15:41:20 2023, max compression
+gzip compressed data, was "bring_order-0.3.1.tar", max compression
```

## Comparing `bring-order-0.2.0.tar` & `bring_order-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,12 @@
-drwxr-xr-x   0 evgeniia  (1000) users      (100)        0 2023-06-19 15:41:20.461287 bring-order-0.2.0/
--rw-r--r--   0 evgeniia  (1000) users      (100)     1067 2023-06-06 06:49:56.000000 bring-order-0.2.0/LICENSE
--rw-r--r--   0 evgeniia  (1000) users      (100)     4407 2023-06-19 15:41:20.461287 bring-order-0.2.0/PKG-INFO
--rw-r--r--   0 evgeniia  (1000) users      (100)     3792 2023-06-19 15:15:00.000000 bring-order-0.2.0/README.md
-drwxr-xr-x   0 evgeniia  (1000) users      (100)        0 2023-06-19 15:41:20.457287 bring-order-0.2.0/bring_order/
--rw-r--r--   0 evgeniia  (1000) users      (100)       46 2023-06-04 16:23:23.000000 bring-order-0.2.0/bring_order/__init__.py
--rw-r--r--   0 evgeniia  (1000) users      (100)     6798 2023-06-19 14:35:03.000000 bring-order-0.2.0/bring_order/bodi.py
--rw-r--r--   0 evgeniia  (1000) users      (100)     3262 2023-06-19 14:35:03.000000 bring-order-0.2.0/bring_order/bogui.py
--rw-r--r--   0 evgeniia  (1000) users      (100)     9124 2023-06-17 06:21:30.000000 bring-order-0.2.0/bring_order/boutils.py
--rw-r--r--   0 evgeniia  (1000) users      (100)     2542 2023-06-18 16:42:54.000000 bring-order-0.2.0/bring_order/bringorder.py
--rw-r--r--   0 evgeniia  (1000) users      (100)     9019 2023-06-19 14:35:03.000000 bring-order-0.2.0/bring_order/deductive.py
--rw-r--r--   0 evgeniia  (1000) users      (100)     7349 2023-06-19 14:35:03.000000 bring-order-0.2.0/bring_order/inductive.py
-drwxr-xr-x   0 evgeniia  (1000) users      (100)        0 2023-06-19 15:41:20.457287 bring-order-0.2.0/bring_order.egg-info/
--rw-r--r--   0 evgeniia  (1000) users      (100)     4407 2023-06-19 15:41:20.000000 bring-order-0.2.0/bring_order.egg-info/PKG-INFO
--rw-r--r--   0 evgeniia  (1000) users      (100)      379 2023-06-19 15:41:20.000000 bring-order-0.2.0/bring_order.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniia  (1000) users      (100)        1 2023-06-19 15:41:20.000000 bring-order-0.2.0/bring_order.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniia  (1000) users      (100)       11 2023-06-19 15:41:20.000000 bring-order-0.2.0/bring_order.egg-info/requires.txt
--rw-r--r--   0 evgeniia  (1000) users      (100)       12 2023-06-19 15:41:20.000000 bring-order-0.2.0/bring_order.egg-info/top_level.txt
--rw-r--r--   0 evgeniia  (1000) users      (100)      529 2023-06-19 15:22:50.000000 bring-order-0.2.0/pyproject.toml
--rw-r--r--   0 evgeniia  (1000) users      (100)       38 2023-06-19 15:41:20.461287 bring-order-0.2.0/setup.cfg
--rw-r--r--   0 evgeniia  (1000) users      (100)     1093 2023-06-19 15:22:17.000000 bring-order-0.2.0/setup.py
+-rw-r--r--   0        0        0     1067 2023-06-26 19:16:39.675135 bring_order-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3792 2023-06-26 19:16:39.675135 bring_order-0.3.1/README.md
+-rw-r--r--   0        0        0       46 2023-06-26 19:16:39.675135 bring_order-0.3.1/bring_order/__init__.py
+-rw-r--r--   0        0        0     7743 2023-06-26 19:16:39.675135 bring_order-0.3.1/bring_order/bodi.py
+-rw-r--r--   0        0        0     3266 2023-06-26 19:16:39.675135 bring_order-0.3.1/bring_order/bogui.py
+-rw-r--r--   0        0        0     9124 2023-06-26 19:16:39.675135 bring_order-0.3.1/bring_order/boutils.py
+-rw-r--r--   0        0        0     2542 2023-06-26 19:16:39.675135 bring_order-0.3.1/bring_order/bringorder.py
+-rw-r--r--   0        0        0    14310 2023-06-26 19:16:39.675135 bring_order-0.3.1/bring_order/deductive.py
+-rw-r--r--   0        0        0    10071 2023-06-26 19:16:39.675135 bring_order-0.3.1/bring_order/inductive.py
+-rw-r--r--   0        0        0        0 2023-06-26 19:16:39.675135 bring_order-0.3.1/bring_order/untitled
+-rw-r--r--   0        0        0      568 2023-06-26 19:17:17.511103 bring_order-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4521 1970-01-01 00:00:00.000000 bring_order-0.3.1/PKG-INFO
```

### Comparing `bring-order-0.2.0/LICENSE` & `bring_order-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bring-order-0.2.0/PKG-INFO` & `bring_order-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: bring-order
-Version: 0.2.0
-Summary: The tool library is aimed at guiding data scientists with their analysis using custom widgets inside Jupyter Notebook.
-Home-page: https://github.com/Order-Team/bring-order/tree/main
-Author: Bring-Order team
-Author-email: example@email.com
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
+Version: 0.3.1
+Summary: 
+Author: BringOrder team
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: display (>=1.0.0,<2.0.0)
+Requires-Dist: invoke (>=2.1.2,<3.0.0)
+Requires-Dist: ipywidgets (>=8.0.6,<9.0.0)
+Requires-Dist: notebook (>=6.5.4,<7.0.0)
+Requires-Dist: npx (>=0.1.1,<0.2.0)
+Requires-Dist: playwright (>=1.35.0,<2.0.0)
+Requires-Dist: py2nb (>=1.0.0,<2.0.0)
+Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # bring-order
 ![GitHub Actions](https://github.com/Order-Team/bring-order/workflows/CI/badge.svg)
 [![codecov](https://codecov.io/gh/Order-team/bring-order/branch/main/graph/badge.svg?token=e8bdd46f-46b0-410c-820b-84ffca9ca53c)](https://codecov.io/gh/Order-team/bring-order)
 [![GitHub](https://img.shields.io/github/license/Order-Team/bring-order)](LICENSE.md)
 
 The tool is aimed at guiding data scientists with their analysis using custom widgets inside Jupyter Notebook.
@@ -176,7 +181,8 @@
 ```
 to run robottests
 
 ```bash
 invoke alltests
 ```
 to run all of the above
+
```

### Comparing `bring-order-0.2.0/README.md` & `bring_order-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bring-order-0.2.0/bring_order/bodi.py` & `bring_order-0.3.1/bring_order/bodi.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         """Class constructor
         """
         self.start_analysis = start_analysis
         self.boutils = boutils
         self.bogui = bogui
         self.cell_count = 0
         self.buttons = self.bogui.init_buttons(self.button_list)
+        self.data_name = self.bogui.create_input_field()
         self.data_description = self.bogui.create_text_area()
         self.add_cells_int = self.bogui.create_int_text()
         self.import_grid = self.data_import_grid()
         self.data_limitations = []
         self.limitation_grid = None
         self.empty_limitations_error = self.bogui.create_error_message()
 
@@ -78,26 +79,26 @@
         self.display_limitations()
 
     def add_limitation(self, _=None):
         """Button function to add new limitation"""
         if self.limitation_grid:
             self.limitation_grid.close()
 
-        self.data_limitations.append(self.bogui.create_text_area('',f'Limitation {len(self.data_limitations)+1}: '))
+        self.data_limitations.append(self.bogui.create_text_area('',f'Limitation {len(self.data_limitations)+1}'))
 
         self.display_limitations()
 
     def display_limitations(self):
         """Shows text boxes and buttons for adding limitations"""
         limitations_label = self.bogui.create_message(
                 value='Identify limitations to the data: what kind of questions cannot be answered with it?')
 
         rows = len(self.data_limitations)
         if rows == 0:
-            self.data_limitations.append(self.bogui.create_text_area('', 'Limitation 1: '))
+            self.data_limitations.append(self.bogui.create_text_area('', 'Limitation 1'))
             rows +=1
 
         grid = GridspecLayout(rows, 1)
 
         for i in range(rows):
             for j in range(1):
                 grid[i, j] = self.data_limitations[i]
@@ -123,61 +124,92 @@
     def call_check_limitation(self):
         """Checks that none of the limitations is empty"""
         for limitation in self.data_limitations:
             if not self.check_limitations(limitation.value):
                 return False
         return True
 
-    def format_limitations_for_markdown(self):
+    def format_limitations(self):
         """Formats limitations for markdown to prevent Javascript error
         
         Returns:
             formatted_limitations (str)
         """
 
-        formatted_limitations = '## Data limitations\\n'
-        for index, item in enumerate(self.data_limitations):
+        formatted_limitations = '## Limitations\\n'
+        for item in self.data_limitations:
             limitation = '<br />'.join(item.value.split('\n'))
-            limitation_text = f'### Limitation {index+1}\\n{limitation}\\n'
+            limitation_text = f'- {limitation}\\n'
             formatted_limitations += limitation_text
 
         return formatted_limitations
 
     def start_analysis_clicked(self, _=None):
         """Button function to start analysis after data preparation"""
         if self.call_check_limitation():
-            text = self.format_limitations_for_markdown()
+            text = self.format_limitations()
             self.boutils.create_markdown_cells_above(1, text=text)
             clear_output(wait=True)
             self.start_analysis()
         else:
             self.empty_limitations_error.value = 'Data limitations cannot be empty'
 
+    def format_data_description(self):
+        """Formats data description for markdown
+        
+        Returns:
+            formatted_text (str)
+        """
+        title = f'# Data: {self.data_name.value}'
+        description = '<br />'.join(self.data_description.value.split('\n'))
+        formatted_text = f'{title}\\n## Description\\n{description}\\n## Import and cleaning'
+
+        return formatted_text
+
     def start_data_import(self, _=None):
         """Creates markdown for data description and shows buttons for data import"""
-        if self.data_description.value == '':
+        if self.data_name.value == '':
+            self.bodi(error='You must name the data set')
+        elif self.data_description.value == '':
             self.bodi(error='You must give some description of the data')
 
         else:
             self.boutils.hide_current_input()
             clear_output(wait=True)
             display(self.import_grid)
 
-            description = '<br />'.join(self.data_description.value.split('\n'))
-            text = f'# Data preparation\\n## Data description\\n{description}\\n## Data import and cleaning'
-            self.boutils.create_markdown_cells_above(1, text=text)
+            self.boutils.create_markdown_cells_above(1, text=self.format_data_description())
             self.cell_count += 1
 
     def bodi(self, error=''):
         """Main function"""
         clear_output(wait=True)
 
-        description_label = self.bogui.create_label('Describe your data:')
+        title = self.bogui.create_message('What kind of data are you using?')
+        data_title_label = self.bogui.create_label('Name of the data set:')
+        description_label = self.bogui.create_label('Description of the data:')
         error_message = self.bogui.create_error_message(error)
 
-        grid = widgets.VBox([
-            widgets.HBox([description_label, self.data_description]),
-            error_message,
-            self.buttons['Save description']
-        ])
+        grid = widgets.AppLayout(
+            header=title,
+            left_sidebar=widgets.VBox([
+                data_title_label,
+                description_label
+            ]),
+            center=widgets.VBox([
+                    self.data_name,
+                    self.data_description
+            ]),
+            footer=widgets.HBox([
+                self.buttons['Save description'],
+                error_message,
+            ]),
+            pane_widths=[1, 5, 0],
+            grid_gap='10px'
+        )
 
         display(grid)
+
+        if 'description' in error:
+            self.data_description.focus()
+        else:
+            self.data_name.focus()
```

### Comparing `bring-order-0.2.0/bring_order/bogui.py` & `bring_order-0.3.1/bring_order/bogui.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         input_field = widgets.Text(value=default_value)
         return input_field
 
     def create_text_area(self, default_value='', place_holder=''):
         """Creates text box"""
         text_area = widgets.Textarea(value=default_value,layout={'width': '70%'}, placeholder=place_holder)
         return text_area
-
+    
     def create_label(self, value):
         """Creates label"""
         label = widgets.Label(value=value,
                               layout=widgets.Layout(justify_content='flex-end'))
         return label
 
     def create_placeholder(self):
```

### Comparing `bring-order-0.2.0/bring_order/boutils.py` & `bring_order-0.3.1/bring_order/boutils.py`

 * *Files identical despite different names*

### Comparing `bring-order-0.2.0/bring_order/bringorder.py` & `bring_order-0.3.1/bring_order/bringorder.py`

 * *Files identical despite different names*

### Comparing `bring-order-0.2.0/bring_order/deductive.py` & `bring_order-0.3.1/bring_order/inductive.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,223 +1,275 @@
-"""Deductive class"""
+"""Class for Inductive analysis"""
 from ipywidgets import widgets
-from IPython.display import display
+from IPython.display import display, clear_output, Javascript
 
-class Deductive:
-    """Class that guides deductive analysis"""
+class Inductive:
+    """Class that guides inductive analysis"""
     def __init__(self, bogui, boutils, start_new):
-        """Class constructor
-        
-        Args:
-            bogui (BOGui)
-            boutils (BOUtils)
-            start_new (function): Function to start new analysis with same data
-        """
-        self.cell_count = 0
-        self.start_new = start_new
+        """Class constructor."""
         self.bogui = bogui
-        self.boutils = boutils
+        self.utils = boutils
+        self.start_new = start_new
+        self.cell_count = 0
         self.buttons = self.bogui.init_buttons(self.button_list)
-        #List of hypotheses: 0 = hypothesis, 1 = null hypothesis
-        self.hypotheses = [self.bogui.create_input_field(), self.bogui.create_input_field()]
-        self.empty_hypo_error = self.bogui.create_error_message()
-        self.empty_null_error = self.bogui.create_error_message()
-        self.hypotheses_grid = self.create_hypotheses_grid()
         self.add_cells_int = self.bogui.create_int_text()
-        self.confirmed_grid = None
+        self.notes = self.bogui.create_text_area()
         self.conclusion = None
-        self.data_limitations = ['Data limitations missing']
-        self.limitation_prompt = None
+        self.summary = self.bogui.create_text_area()
+        self.empty_notes_error = self.bogui.create_error_message()
+        self.observations = []
+        self.new_analysis_view = widgets.HBox([
+            self.buttons['New analysis'],
+            self.buttons['Prepare new data'],
+            self.buttons['All done']]
+        )
+        self.export_view = widgets.HBox([self.buttons['Export to pdf'],
+                                         self.buttons['Close BringOrder']])
 
     @property
     def button_list(self):
-        """Buttons for deductive class.
+        """Buttons for Inductive class.
 
         Returns:
-            list of tuples in format (description: str, command: func, style: str)"""
+            list of tuples in format (description: str, command: func, style: str) """
         button_list = [('Open cells', self.open_cells, 'warning'),
-                       ('Delete last cell', self.delete_last_cell, 'danger'),
-                       ('Save', self.check_data_limitations, 'success'),
-                       ('Clear', self.clear_hypotheses, 'primary'),
-                       ('Yes', self.valid_hypotheses, 'success'),
-                       ('No', self.bad_hypotheses, 'warning'),
-                       ('Run cells', self.run_cells, 'primary'),
-                       ('Clear cells', self.clear_cells, 'danger'),
-                       ('New analysis', self.start_new_analysis, 'success'),
-                       ('Prepare new data', self.start_analysis_with_new_data, 'success'),
-                       ('All done', self.all_done, 'success')]
-        return button_list
-
-    def create_hypotheses_grid(self):
-        """Creates widgets"""
-        hypothesis_label = self.bogui.create_label('Hypothesis:')
-        null_label = self.bogui.create_label('Null hypothesis:')
-        empty = self.bogui.create_placeholder()
-
-        grid = self.bogui.create_grid(5, 2,
-            [empty, self.empty_hypo_error,
-             hypothesis_label, self.hypotheses[0],
-             null_label, self.hypotheses[1],
-             empty, self.empty_null_error,
-             empty, widgets.HBox([self.buttons['Save'], self.buttons['Clear']])
-            ])
-        return grid
-
-    def start_deductive_analysis(self, _=None):
-        """Button function for deductive analysis"""
-        display(self.hypotheses_grid)
-        self.hypotheses[0].focus()
-
-    def check_data_limitations(self, _=None):
-        """Displays the prompt for the check against data limitations"""
-        #print('checking limits: ' + self.data_limitations) #This is for debugging
-        if self.check_hypotheses():
-            limitations = ''.join(f"Limitation {count}: {item.value} <br>" for count, item in enumerate(self.data_limitations, start=1))
-
-            limitation_prompt_text = widgets.HTML(
-                'Do the hypotheses fit within the limitations of the data set?' 
-                + '<br>' + limitations)
-
-            self.limitation_prompt = widgets.VBox([limitation_prompt_text,
-                widgets.HBox([self.buttons['Yes'], self.buttons['No']])
-                ])
-            display(self.limitation_prompt)
-
-    def valid_hypotheses(self, _=None):
-        """Closes the data limitation check prompt and calls save_hypotheses()"""
-        self.limitation_prompt.close()
-        self.save_hypotheses()
-
-    def bad_hypotheses(self, _=None):
-        """Closes the data limitation check prompt and calls clear_hypotheses()"""
-        # TODO: set some error message for a hypothesis that doesn't fit
-        # data limitations and ask the user for a better one
-        self.limitation_prompt.close()
-        self.clear_hypotheses()
-
-    def check_hypotheses(self):
-        """Checks that hypothesis and null hypothesis are not empty.
-
-        Returns:
-            True/False
-        """
-        if len(self.hypotheses[0].value) > 0 and len(self.hypotheses[1].value) > 0:
-            return True
+                   ('Delete last cell', self.delete_last_cell, 'danger'),
+                   ('Clear cells', self.clear_cells, 'danger'),
+                   ('Run cells', self.run_cells, 'primary'),
+                   ('New analysis', self.start_new_analysis, 'success'),
+                   ('Ready to summarize', self.execute_ready, 'primary'),
+                   ('Submit observation', self.new_observation, 'warning'),
+                   ('Submit summary', self.submit_summary, 'success'),
+                   ('Prepare new data', self.prepare_new_data_pressed, 'success'),
+                   ('All done', self.all_done, 'success'),
+                   ('Export to pdf', self.export_to_pdf, 'success'),
+                   ('Close BringOrder', self.no_export, 'success')]
 
-        if self.hypotheses[0].value == '':
-            self.empty_hypo_error.value = 'Hypothesis missing'
-        else:
-            self.empty_hypo_error.value = ''
-
-        if self.hypotheses[1].value == '':
-            self.empty_null_error.value = 'Null hypothesis missing'
-        else:
-            self.empty_null_error.value = ''
-
-        return False
-
-    def save_hypotheses(self, _=None):
-        """Saves hypotheses and displays buttons for running code"""
-        hypotheses = f'- Hypothesis: {self.hypotheses[0].value}\
-        \\n- Null hypothesis: {self.hypotheses[1].value}'
-        text = f'# Deductive analysis\\n## Hypotheses\\n{hypotheses}\\n## Data analysis'
-        if self.check_hypotheses():
-            self.boutils.create_markdown_cells_above(1, text=text)
-            self.confirmed_grid = self.create_confirmed_grid()
-            self.hypotheses_grid.close()
-            display(self.confirmed_grid)
-
-    def clear_hypotheses(self, _=None):
-        """Button function for resetting hypothesis and null hypothesis inputs"""
-        self.hypotheses[0].value = ''
-        self.hypotheses[1].value = ''
-        self.empty_hypo_error.value = ''
-        self.empty_null_error.value = ''
-        self.hypotheses[0].focus()
+        return button_list
 
     def open_cells(self, _=None):
-        """Button function for opening new code cells"""
+        """Open cells button function that opens the selected
+        number of code cells"""
         if self.add_cells_int.value > 0:
             self.cell_count += self.add_cells_int.value
-            self.boutils.create_code_cells_above(self.add_cells_int.value)
+            self.utils.create_code_cells_above(self.add_cells_int.value)
 
     def delete_last_cell(self, _=None):
-        """Button function for deleting the last code cell"""
+        """Delete last cell-button function"""
         if self.cell_count > 0:
-            self.boutils.delete_cell_above()
+            self.utils.delete_cell_above()
             self.cell_count -= 1
 
-    def deactivate_cell_operations(self):
-        """Deactivates buttons after runnig code block"""
-        self.buttons['Open cells'].disabled = True
-        self.buttons['Clear cells'].disabled = True
-        self.buttons['Delete last cell'].disabled = True
+    def clear_cells(self, _=None):
+        """Clears all code cells above."""
+        self.utils.clear_code_cells_above(self.cell_count)
+
+    def buttons_disabled(self, disabled):
+        """Activates/deactivates buttons
+        
+        Args:
+            disbled (bool): True to disable, False to activate
+        """
+
+        self.buttons['Open cells'].disabled = disabled
+        self.buttons['Clear cells'].disabled = disabled
+        self.buttons['Delete last cell'].disabled = disabled
+        self.buttons['Ready to summarize'].disabled = disabled
 
     def run_cells(self, _=None):
-        """Button function"""
-        self.boutils.run_cells_above(
-            self.cell_count)
-        self.deactivate_cell_operations()
+        """Executes cells above and displays text area for observations of analysis."""
+        if self.cell_count == 0:
+            return
 
+        self.utils.run_cells_above(self.cell_count)
         if self.conclusion:
             self.conclusion.close()
 
-        question = self.bogui.create_message(value='What happened?')
-        conclusion_label = self.bogui.create_message(value='Accepted hypothesis:')
-        conclusion = self.bogui.create_radiobuttons(
-            options=[f'Hypothesis: {self.hypotheses[0].value}',
-                     f'Null hypothesis: {self.hypotheses[1].value}'])
-
-        self.conclusion = widgets.AppLayout(
-            header=question,
-            left_sidebar=conclusion_label,
-            center=conclusion,
-            footer=widgets.HBox([
-                self.buttons['New analysis'],
-                self.buttons['Prepare new data'],
-                self.buttons['All done']])
-        )
+        self.buttons_disabled(True)
+
+        notes_label = self.bogui.create_label(value='Explain what you observed:')
+        self.conclusion = widgets.VBox([
+            widgets.HBox([notes_label, self.notes]),
+            self.empty_notes_error,
+            self.buttons['Submit observation']
+        ])
+
         display(self.conclusion)
 
-    def clear_cells(self, _=None):
-        """Clear button function to clear cells above"""
-        self.boutils.clear_code_cells_above(self.cell_count)
+    def get_first_words(self, word_list):
+        """Takes a word list and returns a string that has the first sentence or
+        the first five words and three dots if the sentence is longer.
+        
+        Args:
+            word_list (list)
+            
+        Returns:
+            first_words (str)
+        """
+        first_words = f'{word_list[0]}'
 
-    def create_confirmed_grid(self):
-        """Creates widget grid"""
-        cell_number_label = self.bogui.create_label('Add code cells for your analysis:')
+        for word in word_list[1:5]:
+            first_words += f' {word}'
+            if any(mark in word for mark in ['.', '?', '!']):
+                return first_words.strip('.')
 
-        grid = widgets.GridspecLayout(2, 2, justify_items='center', width='70%', align_items='top')
-        grid[1, 0] = widgets.HBox([cell_number_label, self.add_cells_int])
-        grid[1, 1] = widgets.TwoByTwoLayout(
-            top_left=self.buttons['Open cells'],
-            bottom_left=self.buttons['Run cells'],
-            top_right=self.buttons['Delete last cell'],
-            bottom_right=self.buttons['Clear cells'])
+        first_words.strip('.').strip(',')
+        if len(word_list) > 5:
+            first_words += '...'
 
-        return grid
+        return first_words
+
+    def format_observation(self):
+        """Formats observation for markdown.
+        
+        Returns:
+            formatted_obs (str)
+        """
+        formatted_obs = f'## Observation {len(self.observations)}: '
 
-    def save_results(self):
-        """Prints results and hides widgets"""
-        text = f'## Accepted hypothesis\\n{self.conclusion.center.value}'
-        self.boutils.create_markdown_cells_above(1, text=text)
-        self.confirmed_grid.close()
-        self.conclusion.close()
+        notes_list = self.notes.value.split('\n')
+        first_line_list = notes_list[0].split(' ')
+        first_words = self.get_first_words(first_line_list)
+        formatted_obs += f'{first_words}\\n'
+
+        notes = '<br />'.join(notes_list)
+        formatted_obs += notes
+
+        return formatted_obs
+
+    def new_observation(self, _=None):
+        """Checks new observation, saves it, and resets cell count"""
+        if self.check_notes():
+            self.observations.append(self.notes.value)
+            text = self.format_observation()
+            self.utils.create_markdown_cells_above(1, text=text)
+            self.buttons_disabled(False)
+            self.empty_notes_error.value = ''
+            self.conclusion.close()
+            self.notes.value = ''
+            self.cell_count = 0
+
+        else:
+            self.empty_notes_error.value = 'Observation field can not be empty'
 
     def start_new_analysis(self, _=None):
-        """Button function to save results and star new analysis"""
-        self.save_results()
+        """Starts new bringorder object with old data"""
+        clear_output(wait=True)
         self.start_new()
 
-    def start_analysis_with_new_data(self, _=None):
-        """Button function to start over with new data"""
-        self.save_results()
-        self.boutils.execute_cell_from_current(1, 'BringOrder()')
+    def prepare_new_data_pressed(self, _=None):
+        '''Starts new analysis with importing new data'''
+        self.utils.execute_cell_from_current(0, 'BringOrder()')
+
+    def execute_ready(self, _=None):
+        """Executes code cells after Get summary button is clicked."""
+        clear_output(wait=True)
+        self.display_summary()
+
+    def display_summary(self, error=''):
+        """Prints all observations and asks for summary"""
+        clear_output(wait=True)
+
+        observations = "<ul>\n"
+        observations += "\n".join(["<li>" + observation + "</li>" for observation in self.observations])
+        observations += "\n</ul>"
+
+        observation_list = widgets.HTML(
+            '</br>'+'<h4>All your observations from the data:</h4>'+observations)
+
+        # observation_string = '\n'.join((f"Observation {i+1}: {observation}\n") for i, observation
+        #          in enumerate(self.observations))
+        # text = f'All your observations from the data:\n\n{observation_string}'
+        # print(text)
+
+        summary_label = self.bogui.create_label('What do these observations mean?')
+        error_message = self.bogui.create_error_message(value=error)
+        grid = widgets.VBox([
+            observation_list,
+            widgets.HBox([summary_label, self.summary]),
+            error_message,
+            self.buttons['Submit summary']
+        ])
+        display(grid)
+
+    def format_summary(self):
+        """Formats summary for markdown
+        
+        Returns:
+            formatted_summary (str)
+        """
+        formatted_summary = '## Summary: '
+
+        summary_list = self.summary.value.split('\n')
+        first_line_list = summary_list[0].split(' ')
+        first_words = self.get_first_words(first_line_list)
+        formatted_summary += f'{first_words}\\n'
+
+        summary = '<br />'.join(summary_list)
+        formatted_summary += summary
+
+        return formatted_summary
+
+    def submit_summary(self, _=None):
+        """Button function to submit summary"""
+        if self.summary.value == '':
+            self.display_summary(error='You must write some kind of summary')
+            return
+
+        text = self.format_summary()
+        self.utils.create_markdown_cells_above(1, text=text)
+        clear_output(wait=False)
+        self.new_analysis()
+
+    def check_notes(self):
+        """Checks that text field was filled"""
+        if self.notes.value == '':
+            return False
+        return True
+
+    def create_cell_operations(self):
+        """Displays buttons for operations in inductive analysis"""
+        self.buttons['Ready to summarize'].disabled = True
+        cell_number_label = self.bogui.create_label('Add code cells for your analysis:')
+
+        cell_buttons = widgets.TwoByTwoLayout(
+            top_left=self.buttons['Open cells'],
+            bottom_left=self.buttons['Run cells'],
+            top_right=self.buttons['Delete last cell'],
+            bottom_right=self.buttons['Clear cells']
+        )
+
+        grid = widgets.GridspecLayout(2, 3, height='auto', width='100%')
+        grid[0, 0] = widgets.HBox([cell_number_label, self.add_cells_int])
+        grid[:, 1] = cell_buttons
+        grid[1, 2] = self.buttons['Ready to summarize']
+
+        return grid
 
+    def start_inductive_analysis(self):
+        """Starts inductive analysis"""
+        self.utils.create_markdown_cells_above(1, '# Inductive analysis')
+        display(self.create_cell_operations())
 
     def all_done(self, _=None):
-        """Button function to save results when ready."""
-        self.save_results()
-        self.boutils.delete_cell_from_current(1)
+        """Button function to display the export/close phase."""
+        #self.boutils.delete_cell_from_current(1)
+        self.new_analysis_view.close()
+        display(self.export_view)
+
+    def export_to_pdf(self, _=None):
+        """Button function to export the notebook to pdf."""
+        #os.system('jupyter nbconvert Untitled.ipynb --to pdf')
+        self.export_view.close()
+        display(Javascript('print()'))
+        self.utils.delete_cell_from_current(0)
+
+    def no_export(self, _=None):
+        """Button function to close widgets without exporting."""
+        self.utils.delete_cell_from_current(0)
+
+    def new_analysis(self):
+        """Display buttons to start a new analysis or prepare new data for analysis"""
+        display(self.new_analysis_view)
 
     def __repr__(self):
         return ''
```

### Comparing `bring-order-0.2.0/pyproject.toml` & `bring_order-0.3.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "bring-order"
-version = "0.2.0"
+version = "v0.3.1"
 description = ""
 authors = ["BringOrder team"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pytest = "^7.3.1"
 invoke = "^2.1.2"
 ipywidgets = "^8.0.6"
 display = "^1.0.0"
 notebook = "^6.5.4"
 py2nb = "^1.0.0"
+playwright = "^1.35.0"
+npx = "^0.1.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pylint = "^2.17.4"
 coverage = "^7.2.5"
 robotframework = "^6.0.2"
```

