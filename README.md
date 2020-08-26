# Data-Visualization-using-python-seaborn-plotly-cufflinks-

- Seaborn is a Python data visualization library based on matplotlib. It provides a high-level interface for drawing attractive and informative statistical graphics.
- Different graphs and charts of seaborn library is explained in the seaborn  jupyter notebook.
- Plotly provides online graphing, analytics, and statistics tools for individuals and collaboration, as well as scientific graphing libraries for Python, R, MATLAB, Perl, Julia, - Arduino, and REST.
- To install plotly: pip install plotly
- Cufflinks is the thurd-party wrapper library around Plotly.
- Cufflinks connect plotly with pandas to create graphs and charts of dataframe directly.
- Making plotly and cufflinks offline:
- py.offline.init_notebook_mode(connected=True)
- cf.go_offline()
- Creating a Data Frame:
- df=pd.DataFrame(np.random.randn(100,4),columns=['a','b','c','d'])
- df.iplot()
![newplot](https://user-images.githubusercontent.com/68863028/91259122-b7fdf680-e722-11ea-9f73-42da0efef648.png)
