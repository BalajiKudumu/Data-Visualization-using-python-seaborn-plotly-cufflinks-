# Data-Visualization-using-python-seaborn-plotly-cufflinks-

- Seaborn is a Python data visualization library based on matplotlib. It provides a high-level interface for drawing attractive and informative statistical graphics.
- Different graphs and charts of seaborn library is explained in the seaborn  jupyter notebook.
- Plotly provides online graphing, analytics, and statistics tools for individuals and collaboration, as well as scientific graphing libraries for Python, R, MATLAB, Perl, Julia, - Arduino, and REST.
- To install plotly: pip install plotly
- Cufflinks is the thurd-party wrapper library around Plotly.
- Cufflinks connect plotly with pandas to create graphs and charts of dataframe directly.
##### Making plotly and cufflinks offline:
- py.offline.init_notebook_mode(connected=True)
- cf.go_offline()
##### Creating a Data Frame:
- df=pd.DataFrame(np.random.randn(100,4),columns=['a','b','c','d'])
- df.iplot()


![newplot](https://user-images.githubusercontent.com/68863028/91259122-b7fdf680-e722-11ea-9f73-42da0efef648.png)


- df.iplot(x="a",y="b",mode="markers")


![newplot (1)](https://user-images.githubusercontent.com/68863028/91259763-fb0c9980-e723-11ea-919d-4b14b1e45202.png)



##### Loading Titanic dataset from seaborn inbuilt datasets:
- titanic=sb.load_dataset("titanic")
- titanic.iplot(kind="bar",x='sex',y="survived",xTitle="Gender",yTitle="Survived")


![newplot (2)](https://user-images.githubusercontent.com/68863028/91260132-46bf4300-e724-11ea-831a-e5fd48eac42d.png)


- df.iplot(kind="bar",bargap=0.5)


![newplot (3)](https://user-images.githubusercontent.com/68863028/91260596-66ef0200-e724-11ea-8c45-71854a04a21e.png)


- df.iplot(kind="bar",barmode='stack',bargap=0.5)


![newplot (4)](https://user-images.githubusercontent.com/68863028/91261135-8dad3880-e724-11ea-87c5-99a212e3ec54.png)


- cf.getThemes()
- cf.set_config_file(theme='white')
- df.iplot(kind="barh",bargap=0.5)


![newplot (5)](https://user-images.githubusercontent.com/68863028/91261595-afa6bb00-e724-11ea-9180-f28a1ccaf047.png)


- titanic.iplot(kind="box")


![newplot (6)](https://user-images.githubusercontent.com/68863028/91262155-d533c480-e724-11ea-87c4-15efaac20b94.png)


##### changing line plot into area plot(it takes only either negative or positive values) so adding 4 to make them positive.
- df['a']=df['a']+4
- df['b']=df['b']+4
- df['c']=df['c']+4
- df['d']=df['d']+4
- df.iplot()


![newplot (7)](https://user-images.githubusercontent.com/68863028/91263232-2348c800-e725-11ea-8cb6-e5d7aec939c9.png)


- df.iplot(kind="area")



![newplot (8)](https://user-images.githubusercontent.com/68863028/91264132-63a84600-e725-11ea-98dd-95ed65129206.png)



- df3d=pd.DataFrame({'x':[10,30,28,25],'y':[20,10,30,25],'z':[20,10,28,35]})
- df3d.iplot(kind="surface",colorscale="rdylbu")



![newplot (9)](https://user-images.githubusercontent.com/68863028/91264619-85093200-e725-11ea-9728-860f218b8475.png)


- cf.datagen.sinwave(25,5.34).iplot(kind="surface")


![newplot (10)](https://user-images.githubusercontent.com/68863028/91265475-c0a3fc00-e725-11ea-90ee-50b4b6cf79ed.png)



- cf.datagen.scatter3d(4,100,mode="stocks")
- cf.datagen.scatter3d(4,100,mode="stocks").iplot(kind="scatter3d",x="x",y="y",z="z")



![newplot (11)](https://user-images.githubusercontent.com/68863028/91266086-e8935f80-e725-11ea-9008-c4c7b95f332b.png)


- df[['a','b']].iplot(kind='spread')


![newplot (12)](https://user-images.githubusercontent.com/68863028/91266413-137db380-e726-11ea-80dc-7e1f12c42ba9.png)


- df3d[['x','y']].iplot(kind='spread')


![newplot (13)](https://user-images.githubusercontent.com/68863028/91266477-38722680-e726-11ea-826a-f8d5597a2ec4.png)


- df.iplot(kind="hist",bins=34,barmode="group",bargap=0.5) #barmode= stack or overlay


![newplot (14)](https://user-images.githubusercontent.com/68863028/91266548-60fa2080-e726-11ea-9bf4-55f37371e616.png)


- cf.datagen.bubble3d(5,2,mode="abc").iplot(kind="bubble3d",x='x',y='y',z='z',size="size")


![newplot (15)](https://user-images.githubusercontent.com/68863028/91266615-7e2eef00-e726-11ea-8b31-1ba6b32692d0.png)


- cf.datagen.heatmap(20,20).iplot(kind="heatmap",colorscale="rdylbu",title="cufflinks-heatmap")


![newplot (16)](https://user-images.githubusercontent.com/68863028/91266714-aa4a7000-e726-11ea-9392-871da15b2e61.png)




























