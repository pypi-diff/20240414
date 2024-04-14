# Comparing `tmp/glook-0.0.3a0-py3-none-any.whl.zip` & `tmp/glook-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,14 @@
-Zip file size: 13425 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat     2077 b- defN 24-Mar-25 18:28 glook/GLook.py
+Zip file size: 16102 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat     2776 b- defN 24-Apr-14 16:10 glook/GLook.py
 -rw-rw-rw-  2.0 fat       51 b- defN 24-Mar-25 17:39 glook/__init__.py
 -rw-rw-rw-  2.0 fat      339 b- defN 24-Mar-25 18:24 glook/cli.py
--rw-rw-rw-  2.0 fat    14991 b- defN 24-Mar-26 17:03 glook/pages/2_Univariate_Analysis.py
--rw-rw-rw-  2.0 fat     7721 b- defN 24-Mar-26 18:34 glook/pages/3_Bivariate_Analysis.py
--rw-rw-rw-  2.0 fat     7507 b- defN 24-Mar-26 18:50 glook/pages/4_Trivariate_Analysis.py
--rw-rw-rw-  2.0 fat     3910 b- defN 24-Mar-26 19:01 glook-0.0.3a0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-26 19:01 glook-0.0.3a0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       38 b- defN 24-Mar-26 19:01 glook-0.0.3a0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        6 b- defN 24-Mar-26 19:01 glook-0.0.3a0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      882 b- defN 24-Mar-26 19:01 glook-0.0.3a0.dist-info/RECORD
-11 files, 37614 bytes uncompressed, 11931 bytes compressed:  68.3%
+-rw-rw-rw-  2.0 fat     3698 b- defN 24-Apr-14 11:53 glook/pages/1_General_Data_Insights.py
+-rw-rw-rw-  2.0 fat    17728 b- defN 24-Apr-14 15:18 glook/pages/2_Univariate_Analysis.py
+-rw-rw-rw-  2.0 fat     7771 b- defN 24-Apr-14 11:53 glook/pages/3_Bivariate_Analysis.py
+-rw-rw-rw-  2.0 fat     7596 b- defN 24-Mar-28 17:23 glook/pages/4_Trivariate_Analysis.py
+-rw-rw-rw-  2.0 fat     3928 b- defN 24-Apr-14 16:12 glook-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-14 16:12 glook-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       38 b- defN 24-Apr-14 16:12 glook-0.0.5.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-14 16:12 glook-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      967 b- defN 24-Apr-14 16:12 glook-0.0.5.dist-info/RECORD
+12 files, 44990 bytes uncompressed, 14476 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -3,32 +3,35 @@
 
 Filename: glook/__init__.py
 Comment: 
 
 Filename: glook/cli.py
 Comment: 
 
+Filename: glook/pages/1_General_Data_Insights.py
+Comment: 
+
 Filename: glook/pages/2_Univariate_Analysis.py
 Comment: 
 
 Filename: glook/pages/3_Bivariate_Analysis.py
 Comment: 
 
 Filename: glook/pages/4_Trivariate_Analysis.py
 Comment: 
 
-Filename: glook-0.0.3a0.dist-info/METADATA
+Filename: glook-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: glook-0.0.3a0.dist-info/WHEEL
+Filename: glook-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: glook-0.0.3a0.dist-info/entry_points.txt
+Filename: glook-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: glook-0.0.3a0.dist-info/top_level.txt
+Filename: glook-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: glook-0.0.3a0.dist-info/RECORD
+Filename: glook-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## glook/GLook.py

```diff
@@ -1,74 +1,95 @@
 # pip or conda to install openpyxl.
 # page 1
 import streamlit as st
 import pandas as pd
-
+import numpy as np
+# import matplotlib.pyplot as plt
+# import matplotlib
+# matplotlib.use('TkAgg')
 if "shared" not in st.session_state:
 	st.session_state["shared"] = True
 
 st.title("G-Look Auto EDA")
 # st.write("`")
 gg = st.file_uploader("Input:", type=['csv', 'xlsx'])
 
-df = None
+# df = None
+# if st.button("process", use_container_width=True):
+# 	try:
+# 		# Try reading as CSV
+# 		df = pd.read_csv(gg)
+# 	except:
+# 		try:
+# 			# Try reading as Excel
+# 			df = pd.read_excel(gg, engine='openpyxl')
+# 		except Exception as e:
+# 			st.error(f"Error reading file: {e}")
+# 	# Store the DataFrame in session_state
+# 	st.session_state.df = df
+# 	st.switch_page("pages/2_Univariate_Analysis.py")
+# if gg is not None:
+# 	try:
+# 		# Try reading as CSV
+# 		df = pd.read_csv(gg)
+# 	except:
+# 		try:
+# 			# Try reading as Excel
+# 			df = pd.read_excel(gg, engine='openpyxl')
+# 		except Exception as e:
+# 			# st.error(f"Error reading file: {e}")
+# 			print(e)
+
+# if df is not None:
+# 	# st.dataframe(df)
+# 	# Get number of rows
+# 	num_rows = df.shape[0]
+
+# 	# Get number of columns
+# 	num_columns = df.shape[1]
+
+# 	# Check for duplicates
+# 	num_duplicates = df.duplicated().sum()
+
+# 	# Get memory usage
+# 	memory_usage = df.memory_usage(deep=True).sum() / (1024 * 1024)  # Convert bytes to KB
+
+# 	# Get number of features
+# 	num_features = len(df.columns)
+
+# 	# Get number of categorical features
+# 	num_categorical = len(df.select_dtypes(include=['object']).columns)
+
+# 	# Get number of numerical features
+# 	num_numerical = len(df.select_dtypes(include=['number']).columns)
+
+# 	# Display the insights
+# 	st.subheader(f"Data dimensions: :green[{num_rows} rows, {num_columns} columns]")
+# 	st.subheader(f"Number of rows: :green[{num_rows}]")
+# 	st.subheader(f"Number of duplicates: :green[{num_duplicates}]")
+# 	st.subheader(f"Memory usage: :green[{memory_usage:.5f} KB]")
+# 	st.subheader(f"Number of features: :green[{num_features}]")
+# 	st.subheader(f"Number of categorical features: :green[{num_categorical}]")
+# 	st.subheader(f"Number of numerical features: :green[{num_numerical}]")
+# 	st.dataframe(df)
+
+
 
-if gg is not None:
-	 try:
-		  # Try reading as CSV
-		  df = pd.read_csv(gg)
-	 except:
-			try:
-				# Try reading as Excel
-				df = pd.read_excel(gg)
-			except Exception as e:
-				st.error(f"Error reading file: {e}")
-
-if df is not None:
-	# st.dataframe(df)
-	# Get number of rows
-	num_rows = df.shape[0]
-
-	# Get number of columns
-	num_columns = df.shape[1]
-
-	# Check for duplicates
-	num_duplicates = df.duplicated().sum()
-
-	# Get memory usage
-	memory_usage = df.memory_usage(deep=True).sum() / (1024 * 1024)  # Convert bytes to KB
-
-	# Get number of features
-	num_features = len(df.columns)
-
-	# Get number of categorical features
-	num_categorical = len(df.select_dtypes(include=['object']).columns)
-
-	# Get number of numerical features
-	num_numerical = len(df.select_dtypes(include=['number']).columns)
-
-	# Display the insights
-	st.subheader(f"Data dimensions: :green[{num_rows} rows, {num_columns} columns]")
-	st.subheader(f"Number of rows: :green[{num_rows}]")
-	st.subheader(f"Number of duplicates: :green[{num_duplicates}]")
-	st.subheader(f"Memory usage: :green[{memory_usage:.5f} KB]")
-	st.subheader(f"Number of features: :green[{num_features}]")
-	st.subheader(f"Number of categorical features: :green[{num_categorical}]")
-	st.subheader(f"Number of numerical features: :green[{num_numerical}]")
-	st.dataframe(df)
-else:
-	st.write("DataFrame not yet uploaded.")
+# else:
+# 	st.write("DataFrame not yet uploaded.")
 
+# print(9)
 
 if st.button("process", type='primary', use_container_width=True):
 	try:
 		# Try reading as CSV
 		df = pd.read_csv(gg)
 	except:
 		try:
 			# Try reading as Excel
-			df = pd.read_excel(gg)
+			df = pd.read_excel(gg, engine='openpyxl')
 		except Exception as e:
 			st.error(f"Error reading file: {e}")
 	# Store the DataFrame in session_state
 	st.session_state.df = df
-	st.switch_page("pages\\2_Univariate_Analysis.py")
+	st.switch_page("pages/1_General_Data_Insights.py")
+	# st.switch_page("pages/2_Univariate_Analysis.py")
```

## glook/pages/2_Univariate_Analysis.py

```diff
@@ -1,166 +1,176 @@
 # page2.py
-import streamlit as st
-st.set_page_config(
-		page_title="ML-Automation", 
-		page_icon="🏗️", 
-		layout="wide", 
-		initial_sidebar_state = "expanded")
-
-import pandas as pd
-import seaborn as sns
-import matplotlib.pyplot as plt
-import plotly.express as px
-import plotly.graph_objects as go
-import numpy as np
-import statsmodels.api as sm
-st.set_option('deprecation.showPyplotGlobalUse', False)
-from wordcloud import WordCloud
-import matplotlib.pyplot as plt
+try:
+	import streamlit as st
+	st.set_page_config(
+			page_title="ML-Automation", 
+			page_icon="🏗️", 
+			layout="wide", 
+			initial_sidebar_state = "expanded")
+
+	import pandas as pd
+	import seaborn as sns
+	import matplotlib.pyplot as plt
+	import plotly.express as px
+	import plotly.graph_objects as go
+	import numpy as np
+	import statsmodels.api as sm
+	st.set_option('deprecation.showPyplotGlobalUse', False)
+	import matplotlib
+	matplotlib.use('Agg')
+except Exception as e:
+	print("z", e)
 
+# from wordcloud import WordCloud
+# import matplotlib.pyplot as plt
+# import matplotlib
+# matplotlib.use('TkAgg')
 # st.title("1️⃣Univariate Analysis")
 
-try:
-	st.write("Session State:->", st.session_state["shared"])
-	# st.session_state["shared"]
-	# Function to limit the number of unique values for a categorical column
-	def limit_unique_values(series, limit=20):
-		if series.nunique() > limit:
-			top_categories = series.value_counts().index[:limit]
-			return series.apply(lambda x: x if x in top_categories else 'Other')
-		else:
-			return series
 
-	def limit_unique_values_cloud(series, limit=200):
-		if series.nunique() > limit:
-			top_categories = series.value_counts().index[:limit]
-			return top_categories
-		else:
-			return series.unique()
-
-	# def limit_unique_values_cloud(series, limit=200):
-	# 	if series.nunique() > limit:
-	# 		top_categories = series.value_counts().index[:limit]
-	# 		return series.apply(lambda x: x if x in top_categories else 'Other')
-	# 	else:
-	# 		return series
+st.write("Session State:->", st.session_state["shared"])
+# st.session_state["shared"]
+# Function to limit the number of unique values for a categorical column
+def limit_unique_values(series, limit=20):
+	if series.nunique() > limit:
+		top_categories = series.value_counts().index[:limit]
+		return series.apply(lambda x: x if x in top_categories else 'Other')
+	else:
+		return series
 
+def limit_unique_values_cloud(series, limit=200):
+	if series.nunique() > limit:
+		top_categories = series.value_counts().index[:limit]
+		return top_categories
+	else:
+		return series.unique()
 
+# def limit_unique_values_cloud(series, limit=200):
+# 	if series.nunique() > limit:
+# 		top_categories = series.value_counts().index[:limit]
+# 		return series.apply(lambda x: x if x in top_categories else 'Other')
+# 	else:
+# 		return series
 
-	def calculate_insights(column_data):
-	    insights = {}
 
-	    # Count of distinct values
-	    insights['Distinct'] = len(column_data.dropna().unique())
 
-	    # Percentage of distinct values
-	    insights['Distinct (%)'] = len(column_data.dropna().unique()) / len(column_data.dropna()) * 100
+def calculate_insights(column_data):
+	insights = {}
 
-	    # Count of missing values
-	    insights['Missing'] = column_data.isnull().sum()
+	# Count of distinct values
+	insights['Distinct'] = len(column_data.dropna().unique())
 
-	    # Percentage of missing values
-	    insights['Missing (%)'] = column_data.isnull().sum() / len(column_data) * 100
+	# Percentage of distinct values
+	insights['Distinct (%)'] = len(column_data.dropna().unique()) / len(column_data.dropna()) * 100
 
-	    # Count of infinite values
-	    insights['Infinite'] = np.isinf(column_data).sum()
+	# Count of missing values
+	insights['Missing'] = column_data.isnull().sum()
 
-	    # Percentage of infinite values
-	    insights['Infinite (%)'] = np.isinf(column_data).sum() / len(column_data) * 100
+	# Percentage of missing values
+	insights['Missing (%)'] = column_data.isnull().sum() / len(column_data) * 100
 
-	    # Mean
-	    insights['Mean'] = column_data.mean()
+	# Count of infinite values
+	insights['Infinite'] = np.isinf(column_data).sum()
 
-	    # Median
-	    insights['Median'] = column_data.median()
+	# Percentage of infinite values
+	insights['Infinite (%)'] = np.isinf(column_data).sum() / len(column_data) * 100
 
-	    # Mode
-	    insights['Mode'] = column_data.mode().iloc[0]
+	# Mean
+	insights['Mean'] = column_data.mean()
 
-	    # Minimum
-	    insights['Minimum'] = column_data.min()
+	# Median
+	insights['Median'] = column_data.median()
 
-	    # Maximum
-	    insights['Maximum'] = column_data.max()
+	# Mode
+	insights['Mode'] = column_data.mode().iloc[0]
 
-	    # Zeros count
-	    insights['Zeros'] = (column_data == 0).sum()
+	# Minimum
+	insights['Minimum'] = column_data.min()
 
-	    # Percentage of zeros
-	    insights['Zeros (%)'] = (column_data == 0).sum() / len(column_data) * 100
+	# Maximum
+	insights['Maximum'] = column_data.max()
 
-	    # Negative values count
-	    insights['Negative'] = (column_data < 0).sum()
+	# Zeros count
+	insights['Zeros'] = (column_data == 0).sum()
 
-	    # Percentage of negative values
-	    insights['Negative (%)'] = (column_data < 0).sum() / len(column_data) * 100
+	# Percentage of zeros
+	insights['Zeros (%)'] = (column_data == 0).sum() / len(column_data) * 100
 
-	    # Memory size
-	    insights['Memory size'] = column_data.memory_usage(deep=True)
+	# Negative values count
+	insights['Negative'] = (column_data < 0).sum()
 
-	    # 5th percentile
-	    insights['5-th percentile'] = np.percentile(column_data.dropna(), 5)
+	# Percentage of negative values
+	insights['Negative (%)'] = (column_data < 0).sum() / len(column_data) * 100
 
-	    # Q1 (25th percentile)
-	    insights['Q1'] = np.percentile(column_data.dropna(), 25)
+	# Memory size
+	insights['Memory size'] = column_data.memory_usage(deep=True)
 
-	    # Median
-	    insights['Median'] = np.median(column_data.dropna())
+	# 5th percentile
+	insights['5-th percentile'] = np.percentile(column_data.dropna(), 5)
 
-	    # Q3 (75th percentile)
-	    insights['Q3'] = np.percentile(column_data.dropna(), 75)
+	# Q1 (25th percentile)
+	insights['Q1'] = np.percentile(column_data.dropna(), 25)
 
-	    # 95th percentile
-	    insights['95-th percentile'] = np.percentile(column_data.dropna(), 95)
+	# Median
+	insights['Median'] = np.median(column_data.dropna())
 
-	    # Range
-	    insights['Range'] = insights['Maximum'] - insights['Minimum']
+	# Q3 (75th percentile)
+	insights['Q3'] = np.percentile(column_data.dropna(), 75)
 
-	    # Interquartile range (IQR)
-	    insights['Interquartile range'] = insights['Q3'] - insights['Q1']
+	# 95th percentile
+	insights['95-th percentile'] = np.percentile(column_data.dropna(), 95)
 
-	    # Descriptive statistics
-	    insights['Descriptive statistics'] = column_data.describe()
+	# Range
+	insights['Range'] = insights['Maximum'] - insights['Minimum']
 
-	    # Standard deviation
-	    insights['Standard deviation'] = column_data.std()
+	# Interquartile range (IQR)
+	insights['Interquartile range'] = insights['Q3'] - insights['Q1']
 
-	    # Coefficient of variation (CV)
-	    insights['Coefficient of variation (CV)'] = insights['Standard deviation'] / insights['Mean']
+	# Descriptive statistics
+	insights['Descriptive statistics'] = column_data.describe()
 
-	    # Kurtosis
-	    insights['Kurtosis'] = column_data.kurtosis()
+	# Standard deviation
+	insights['Standard deviation'] = column_data.std()
 
-	    # Median Absolute Deviation (MAD)
-	    mad = np.median(np.abs(column_data.dropna() - np.median(column_data.dropna())))
-	    insights['Median Absolute Deviation (MAD)'] = mad
+	# Coefficient of variation (CV)
+	insights['Coefficient of variation (CV)'] = insights['Standard deviation'] / insights['Mean']
 
-	    # Skewness
-	    insights['Skewness'] = column_data.skew()
+	# Kurtosis
+	insights['Kurtosis'] = column_data.kurtosis()
 
-	    # Sum
-	    insights['Sum'] = column_data.sum()
+	# Median Absolute Deviation (MAD)
+	mad = np.median(np.abs(column_data.dropna() - np.median(column_data.dropna())))
+	insights['Median Absolute Deviation (MAD)'] = mad
 
-	    # Variance
-	    insights['Variance'] = column_data.var()
+	# Skewness
+	insights['Skewness'] = column_data.skew()
 
-	    # Monotonicity (not calculated)
+	# Sum
+	insights['Sum'] = column_data.sum()
 
-	    return insights
+	# Variance
+	insights['Variance'] = column_data.var()
 
+	# Monotonicity (not calculated)
 
+	return insights
 
 
+# if "df" in st.session_state:
+# 	df = st.session_state.df
 
 
 
+try:
 	# Assuming df is already defined and stored in session_state
-	if "df" in st.session_state:
+	
+	if "df" in st.session_state and st.session_state.df is not None:
 		df = st.session_state.df
-		
+		# import time
+		# s = time.time()
 		# # Get number of rows
 		# num_rows = df.shape[0]
 		
 		# # Get number of columns
 		# num_columns = df.shape[1]
 		
 		# # Check for duplicates
@@ -185,40 +195,76 @@
 		# st.subheader(f"Number of features: :green[{num_features}]")
 		# st.subheader(f"Number of categorical features: :green[{num_categorical}]")
 		# st.subheader(f"Number of numerical features: :green[{num_numerical}]")
 		
 		# Display insights for each column
 		st.title("1️⃣ Univariate Analysis")
 		# st.header(":green[Column Insights:]⤵️")
+		# html_content = ""
 		for idx, column in enumerate(df.columns):
-			st.subheader(f":green[**Column {idx + 1}:** {column}]")
+			# st.subheader(f':green[**Column {idx + 1}:** {column}]')
+			# subh = f""":green[Column {idx + 1}: {column}]"""
+			# st.subheader(subh)
+			# subh = f"**Column {idx + 1}:** `{column}`"
+			# st.markdown(subh, unsafe_allow_html=True)
+			# subh = "**Column " + str(idx + 1) + ":** `" + column + "`"
+			# st.markdown(subh, unsafe_allow_html=True)
+			html_content = f"<div class='column-header'>Column {idx + 1}: <code>{column}</code></div>"
+
+			css_style = """
+			<style>
+			.column-header {
+				margin-bottom: 10px;
+				font-weight: bold;
+				font-size: 26px;
+				color: green; /* Change color as needed */
+			}
+			</style>
+			"""
+
+			# Embed HTML and CSS code into Streamlit
+			st.markdown(css_style, unsafe_allow_html=True)
+			st.markdown(html_content, unsafe_allow_html=True)
 			if df[column].dtype == 'object':
 				col1, col2 = st.columns(2)
 				with col1:
 					unique_values = df[column].nunique()
 					st.write(f"  - Data Type: :green[{df[column].dtype}]")
 					st.write(f"  - Number of Unique Values: :green[{unique_values}]")
 					if unique_values <= 20:
 						st.write(f"  - Unique Values: :green[{', '.join(map(str, df[column].unique()))}]")
 					else:
 						st.write(f"  - Top 20 Unique Values:")
 						st.write(f":green[{', '.join(map(str, df[column].value_counts().head(20).index))}]")
 				with col2:
-					""" distinct plot """
+					# """ distinct plot """
 					plt.figure(figsize=(10, 6))  # Adjust figure size
 					try:
 						sns.countplot(x=limit_unique_values(df[column]), data=df, color="green")
 					except:
 						sns.countplot(x=df[column], data=df, color="green")
 					plt.xticks(rotation=45)  # Rotate x-axis labels
 					st.pyplot()
 					plt.close()
+	 				# Assuming df is your DataFrame and column is the specific column you want to plot
+					# def distinct_plot(df, column):
+					# 	try:
+					# 		fig = px.histogram(df, x=limit_unique_values(df[column]), color_discrete_sequence=["green"])
+					# 	except:
+					# 		fig = px.histogram(df, x=df[column], color_discrete_sequence=["green"])
+						
+					# 	fig.update_layout(xaxis_tickangle=-45)  # Rotate x-axis labels
+					# 	st.plotly_chart(fig, use_container_width=True)
+
+					# # Call the function with your DataFrame and column
+					# distinct_plot(df, column)
 				with st.expander("More Info"):
 					# st.write("More Info ⬇")
-					tab1, tab2, tab3 = st.tabs(["Insights", "Donut chart", "WordCloud"])
+					# tab1, tab2, tab3 = st.tabs(["Insights", "Donut chart", "WordCloud"])
+					tab1, tab2 = st.tabs(["Insights", "Donut chart"])
 					with tab1:
 						col7, col8, col9 = st.columns(3)
 						with col7:
 							# Insights
 							st.write("## Insights")
 							approximate_distinct_count = df[column].nunique()
 							approximate_unique_percent = (approximate_distinct_count / len(df)) * 100
@@ -255,64 +301,94 @@
 						data = limit_unique_values(df[column]).value_counts().reset_index()
 						data.columns = [column, 'count']
 
 						fig = px.pie(data, values='count', names=column, hole=0.5)
 						fig.update_traces(textposition='inside', textinfo='percent+label')
 						fig.update_layout(legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1))
 						st.plotly_chart(fig)
-
+						print("j")
 						# st.header("An owl")
 						# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
 
-					with tab3:
-						# Concatenate all values of the column into a single string
-						cleanstrng = ' '.join(df[column].dropna())
-
-						# Check if there are words to plot
-						if cleanstrng:
-							# Generate word cloud
-							word_freq = pd.Series(cleanstrng.split()).value_counts()
+					# with tab3:
+					# 	# Concatenate all values of the column into a single string
+					# 	cleanstrng = ' '.join(df[column].dropna())
+
+					# 	# Check if there are words to plot
+					# 	if cleanstrng:
+					# 		# Generate word cloud
+					# 		word_freq = pd.Series(cleanstrng.split()).value_counts()
 							
-							# Select top 200 words if available, otherwise take the exact number of words
-							if len(word_freq) >= 50:
-								top_words = word_freq.head(50)
-							else:
-								top_words = word_freq
+					# 		# Select top 200 words if available, otherwise take the exact number of words
+					# 		if len(word_freq) >= 50:
+					# 			top_words = word_freq.head(50)
+					# 		else:
+					# 			top_words = word_freq
 
-							words_dict = top_words.to_dict()
+					# 		words_dict = top_words.to_dict()
 							
-							try:
-								# Generate word cloud from frequencies
-								wordcloud_ip = WordCloud(background_color='white', width=2800, height=2400).generate_from_frequencies(words_dict)
-
-								# Display word cloud
-								plt.figure(figsize=(10, 7))
-								plt.imshow(wordcloud_ip, interpolation='bilinear')
-								plt.title(f'Word Cloud for {column}')
-								plt.axis('off')
-								plt.show()
-								st.pyplot(plt, use_container_width=True)
-							except Exception as e:
-								st.write(f"Error generating word cloud: {e}")
-						else:
-							st.write(f"No words to plot for column '{column}'")
+					# 		try:
+					# 			# Generate word cloud from frequencies
+					# 			wordcloud_ip = WordCloud(background_color='white', width=2800, height=2400).generate_from_frequencies(words_dict)
+
+					# 			# Display word cloud
+					# 			plt.figure(figsize=(10, 7))
+					# 			plt.imshow(wordcloud_ip, interpolation='bilinear')
+					# 			plt.title(f'Word Cloud for {column}')
+					# 			plt.axis('off')
+					# 			plt.show()
+					# 			st.pyplot(plt, use_container_width=True)
+					# 		except Exception as e:
+					# 			st.write(f"Error generating word cloud: {e}")
+					# 	else:
+					# 		st.write(f"No words to plot for column '{column}'")
+					
 			elif pd.api.types.is_numeric_dtype(df[column]):
+				print("0a")
 				col3, col4 = st.columns(2)
 				with col3:
+					print("a")
 					st.write(f"  - Data Type: :green[{df[column].dtype}]")
+					print("b")
 					st.write(f"  - Mean: :green[{df[column].mean()}]")
 					st.write(f"  - Standard Deviation: :green[{df[column].std()}]")
 					st.write(f"  - Min Value: :green[{df[column].min()}]")
 					st.write(f"  - Max Value: :green[{df[column].max()}]")
 				with col4:
-					""" KDE plot """
+					# """ KDE plot """
 					plt.figure(figsize=(10, 6))  # Adjust figure size
 					sns.histplot(df[column], kde=True, color="green")
 					st.pyplot()
 					plt.close()
+	 				# KDE plot using Plotly
+					# fig = px.histogram(df, x=df[column], marginal="rug", nbins=30, histnorm='probability density', 
+                  	#  title="KDE Plot", color_discrete_sequence=['green'])
+					# # Create KDE plot using Plotly
+					# # Show the plot using Streamlit
+					# st.plotly_chart(fig, use_container_width=True)
+						# Create KDE plot using Plotly Express
+					# fig = px.histogram(df, x=df[column], marginal="rug", nbins=30, histnorm='probability density', 
+					# 				title="KDE Plot", color_discrete_sequence=['green'],opacity=0.5)
+
+					# # Add labels and annotations
+					# fig.update_layout(
+					# 	xaxis_title=column,
+					# 	yaxis_title="Density",
+					# 	showlegend=False,
+					# 	autosize=True,
+					# 	width=800,
+					# 	height=500,
+					# 	margin=dict(l=40, r=40, t=40, b=40),
+					# )
+
+					# # Customize the appearance of the KDE plot
+					# fig.update_traces(marker=dict(opacity=0.5))
+
+					# # Display the plot using Streamlit
+					# st.plotly_chart(fig, use_container_width=True)
 				with st.expander("More Info"):
 					# st.write("The chart above shows some numbers I picked for you.")
 					tab1, tab2, tab3 = st.tabs(["Insights", "Box plot", "QQ plot"])
 					with tab1:
 						# st.header("An owl")
 						# st.image("https://static.streamlit.io/examples/owl.jpg", width=200)
 						col4, col5, col6 = st.columns(3)
@@ -401,25 +477,33 @@
 							},
 							'showlegend': False,
 							'width': 800,
 							'height': 700,
 						})
 
 						st.plotly_chart(fig)
-					   
-			st.write("---")
+		# st.text("hi")
+		# et = time.time()
+		# tt = et - s
+		# st.text(tt)
+			# st.write("hehe")
 	else:
 		st.write("DataFrame not found.")
 
-	st.write("``")
+		# st.write("``")
 
-except ZeroDivisionError:
+except ZeroDivisionError as ee:
+	print("ee", ee)
+	pass
+except AttributeError as eee:
+	print(eee)
 	pass
 except Exception as e:
 	# handle_error(e)
-    st.error(e)
-    st.subheader("⚠️Please uploade File⚠️")
-    pass
+	st.error(e)
+	st.subheader("⚠️Please uploade File⚠️")
+	print("f", e)
+	pass
```

## glook/pages/3_Bivariate_Analysis.py

```diff
@@ -1,13 +1,15 @@
 # page2.py
 import streamlit as st
 import pandas as pd
 from scipy.stats import zscore
 import plotly.express as px
 import plotly.graph_objects as go
+# import matplotlib
+# matplotlib.use('TkAgg')
 st.title("2️⃣ Bivariate Analysis")
 try:
     st.write("Session State:->", st.session_state["shared"])
     # Access the DataFrame from session_state
     if "df" in st.session_state:
         df = st.session_state.df
         # st.dataframe(df)
@@ -183,15 +185,15 @@
 correlation_matrix = numeric_df.corr()
 
 # Create the heatmap plot
 fig = go.Figure(data=go.Heatmap(
     z=correlation_matrix.values,
     x=correlation_matrix.columns,
     y=correlation_matrix.index,
-    colorscale='Blues',  # You can choose any colorscale
+    colorscale='aggrnyl',  # You can choose any colorscale
 ))
 
 # Add title and axis labels
 fig.update_layout(
     title='Correlation Coefficient Heatmap',
     xaxis=dict(title='Columns'),
     yaxis=dict(title='Columns'),
```

## glook/pages/4_Trivariate_Analysis.py

```diff
@@ -2,14 +2,17 @@
 import streamlit as st
 import pandas as pd
 from scipy.stats import zscore
 import plotly.express as px
 import plotly.graph_objects as go
 import numpy as np
 import plotly.figure_factory as ff
+# import matplotlib.pyplot as plt
+# import matplotlib
+# matplotlib.use('TkAgg')
 st.title("3️⃣ Trivariate Analysis")
 try:
     st.write("Session State:->", st.session_state["shared"])
     # Access the DataFrame from session_state
     if "df" in st.session_state:
         df = st.session_state.df
         # st.dataframe(df)
@@ -192,14 +195,17 @@
         filtered_dff = dff[[x_axis_column, y_axis_column, z_axis_column]].replace([np.inf, -np.inf], np.nan).dropna()
 
         # Add histogram data
         hist_data = [filtered_dff[x_axis_column], filtered_dff[y_axis_column], filtered_dff[z_axis_column]]
         group_labels = ['X-Axis Column', 'Y-Axis Column', 'Z-Axis Column']
         fig = ff.create_distplot(hist_data, group_labels, bin_size=[.1, .25, .5])
         st.plotly_chart(fig, use_container_width=True)
+
+
+
     # Button to show the plot in full-screen mode
     if st.button("Show Full Screen"):
         fig.show()
 
     
 except Exception as e:
     st.error(e)
```

## Comparing `glook-0.0.3a0.dist-info/METADATA` & `glook-0.0.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glook
-Version: 0.0.3a0
+Version: 0.0.5
 Summary: Auto EDA.
 Home-page: https://github.com/gaurang157/glook
 Author: Gaurang Ingle
 Author-email: gaurang.ingle@gmail.com
 Maintainer: Gaurang Ingle
 Maintainer-email: gaurang.ingle@gmail.com
 License: MIT
@@ -67,14 +67,15 @@
 - Visualize distributions of individual columns using:
   - Histograms
   - Box plots
   - Q-Q plot
 
 
 ### Bivariate Analysis
+- Correlation Plot
 - Explore relationships between two columns using:
   - Scatter plots
   - Line plots
   - Bar plots
   - Histograms
   - Box plots
   - Violin plots
```

## Comparing `glook-0.0.3a0.dist-info/RECORD` & `glook-0.0.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-glook/GLook.py,sha256=E2uWuolQ3yl13NoZbAyd9qtMaTUeuJpgP34angrmRjE,2077
+glook/GLook.py,sha256=8ppiVKtPyvA29zKzbQMNHzsM37EltchjN70XrB4AcvA,2776
 glook/__init__.py,sha256=8NahmY4XQHJYMnFDvkZnHpjVBHwxrYrnDFlTTuyXbB0,51
 glook/cli.py,sha256=zBVCZyNNyRj_Zy4Tdnbrb1TrgRhEqAEEdZbk_vrLmi4,339
-glook/pages/2_Univariate_Analysis.py,sha256=zwng9Qp0haOz2BHY4Q6Sf9K2UULwQYBk1RaDL4ifhjo,14991
-glook/pages/3_Bivariate_Analysis.py,sha256=lbX5mc7pbxWz6PhG4c5wZP9C5zDeTacM4Wv3RM50dCk,7721
-glook/pages/4_Trivariate_Analysis.py,sha256=_4GjQVdTo_k1AnvtrIvzOBVYFAD5wHCWymIYYm3kcDk,7507
-glook-0.0.3a0.dist-info/METADATA,sha256=N4AFwNwzYevDrWFn-r4TnCy55w888uDiEMmtROTqCzo,3910
-glook-0.0.3a0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-glook-0.0.3a0.dist-info/entry_points.txt,sha256=7q8WVzTgIl4vX4wJgctmfdJckoB5yPtI0p3hqAQSiFA,38
-glook-0.0.3a0.dist-info/top_level.txt,sha256=2wtpfrIqw9VT_LFDxpI77DArLrUaNjWxyClToM3P9WE,6
-glook-0.0.3a0.dist-info/RECORD,,
+glook/pages/1_General_Data_Insights.py,sha256=btHs2krtxH-H2MdX_x0hLnp8NR38dYvNnVdnNNjZosc,3698
+glook/pages/2_Univariate_Analysis.py,sha256=iQd1MsSFCdtIFU6coQBN-T9FWTVoVUA_Baf1evwjanA,17728
+glook/pages/3_Bivariate_Analysis.py,sha256=0fyPduQDUnlrfYk48YTV3JkxCaTxBjZANfzfPZMjllg,7771
+glook/pages/4_Trivariate_Analysis.py,sha256=Fhkmzqur1xBLPBviyI8kQeeFQbQYAhKwsOLw4E83Hs8,7596
+glook-0.0.5.dist-info/METADATA,sha256=AgSBSMp_djVYw_AefskEm6caHUiNVjz6E4hJqwoEo4w,3928
+glook-0.0.5.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+glook-0.0.5.dist-info/entry_points.txt,sha256=7q8WVzTgIl4vX4wJgctmfdJckoB5yPtI0p3hqAQSiFA,38
+glook-0.0.5.dist-info/top_level.txt,sha256=2wtpfrIqw9VT_LFDxpI77DArLrUaNjWxyClToM3P9WE,6
+glook-0.0.5.dist-info/RECORD,,
```

