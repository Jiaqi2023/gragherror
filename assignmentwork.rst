.. code:: ipython3

    !pip install yfinance==0.1.67
    !mamba install bs4==4.10.0 -y
    !pip install nbformat==4.2.0


.. parsed-literal::

    Requirement already satisfied: yfinance==0.1.67 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (0.1.67)
    Requirement already satisfied: pandas>=0.24 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from yfinance==0.1.67) (1.3.5)
    Requirement already satisfied: numpy>=1.15 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from yfinance==0.1.67) (1.21.6)
    Requirement already satisfied: requests>=2.20 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from yfinance==0.1.67) (2.29.0)
    Requirement already satisfied: multitasking>=0.0.7 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from yfinance==0.1.67) (0.0.11)
    Requirement already satisfied: lxml>=4.5.1 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from yfinance==0.1.67) (4.9.2)
    Requirement already satisfied: python-dateutil>=2.7.3 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from pandas>=0.24->yfinance==0.1.67) (2.8.2)
    Requirement already satisfied: pytz>=2017.3 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from pandas>=0.24->yfinance==0.1.67) (2023.3)
    Requirement already satisfied: charset-normalizer<4,>=2 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from requests>=2.20->yfinance==0.1.67) (3.1.0)
    Requirement already satisfied: idna<4,>=2.5 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from requests>=2.20->yfinance==0.1.67) (3.4)
    Requirement already satisfied: urllib3<1.27,>=1.21.1 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from requests>=2.20->yfinance==0.1.67) (1.26.15)
    Requirement already satisfied: certifi>=2017.4.17 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from requests>=2.20->yfinance==0.1.67) (2022.12.7)
    Requirement already satisfied: six>=1.5 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from python-dateutil>=2.7.3->pandas>=0.24->yfinance==0.1.67) (1.16.0)
    
                      __    __    __    __
                     /  \  /  \  /  \  /  \
                    /    \/    \/    \/    \
    ███████████████/  /██/  /██/  /██/  /████████████████████████
                  /  / \   / \   / \   / \  \____
                 /  /   \_/   \_/   \_/   \    o \__,
                / _/                       \_____/  `
                |/
            ███╗   ███╗ █████╗ ███╗   ███╗██████╗  █████╗
            ████╗ ████║██╔══██╗████╗ ████║██╔══██╗██╔══██╗
            ██╔████╔██║███████║██╔████╔██║██████╔╝███████║
            ██║╚██╔╝██║██╔══██║██║╚██╔╝██║██╔══██╗██╔══██║
            ██║ ╚═╝ ██║██║  ██║██║ ╚═╝ ██║██████╔╝██║  ██║
            ╚═╝     ╚═╝╚═╝  ╚═╝╚═╝     ╚═╝╚═════╝ ╚═╝  ╚═╝
    
            mamba (1.4.2) supported by @QuantStack
    
            GitHub:  https://github.com/mamba-org/mamba
            Twitter: https://twitter.com/QuantStack
    
    █████████████████████████████████████████████████████████████
    
    
    Looking for: ['bs4==4.10.0']
    
    [?25l[2K[0G[+] 0.0s
    [2K[1A[2K[0G[+] 0.1s
    pkgs/main/linux-64 [90m━━━━━━━━━━━━╸[0m[33m━━━━━━━━━━━━[0m   0.0 B /  ??.?MB @  ??.?MB/s  0.1s
    pkgs/main/noarch   [90m━━━╸[0m[33m━━━━━━━━━━━━━━━╸[0m[90m━━━━━[0m   0.0 B /  ??.?MB @  ??.?MB/s  0.1s
    pkgs/r/linux-64    [90m━╸[0m[33m━━━━━━━━━━━━━━━╸[0m[90m━━━━━━━[0m   0.0 B /  ??.?MB @  ??.?MB/s  0.1s
    pkgs/r/noarch      [33m━━━━━━━╸[0m[90m━━━━━━━━━━━━━━━━━[0m   0.0 B /  ??.?MB @  ??.?MB/s  0.1s[2K[1A[2K[1A[2K[1A[2K[1A[2K[0Gpkgs/main/noarch                                              No change
    pkgs/main/linux-64                                            No change
    pkgs/r/noarch                                                 No change
    pkgs/r/linux-64                                               No change
    [?25h
    Pinned packages:
      - python 3.7.*
    
    
    Transaction
    
      Prefix: /home/jupyterlab/conda/envs/python
    
      All requested packages already installed
    
    [?25l[2K[0G[?25hRequirement already satisfied: nbformat==4.2.0 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (4.2.0)
    Requirement already satisfied: ipython-genutils in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from nbformat==4.2.0) (0.2.0)
    Requirement already satisfied: jsonschema!=2.5.0,>=2.4 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from nbformat==4.2.0) (4.17.3)
    Requirement already satisfied: jupyter-core in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from nbformat==4.2.0) (4.12.0)
    Requirement already satisfied: traitlets>=4.1 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from nbformat==4.2.0) (5.9.0)
    Requirement already satisfied: attrs>=17.4.0 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from jsonschema!=2.5.0,>=2.4->nbformat==4.2.0) (23.1.0)
    Requirement already satisfied: importlib-metadata in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from jsonschema!=2.5.0,>=2.4->nbformat==4.2.0) (4.11.4)
    Requirement already satisfied: importlib-resources>=1.4.0 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from jsonschema!=2.5.0,>=2.4->nbformat==4.2.0) (5.12.0)
    Requirement already satisfied: pkgutil-resolve-name>=1.3.10 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from jsonschema!=2.5.0,>=2.4->nbformat==4.2.0) (1.3.10)
    Requirement already satisfied: pyrsistent!=0.17.0,!=0.17.1,!=0.17.2,>=0.14.0 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from jsonschema!=2.5.0,>=2.4->nbformat==4.2.0) (0.19.3)
    Requirement already satisfied: typing-extensions in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from jsonschema!=2.5.0,>=2.4->nbformat==4.2.0) (4.5.0)
    Requirement already satisfied: zipp>=3.1.0 in /home/jupyterlab/conda/envs/python/lib/python3.7/site-packages (from importlib-resources>=1.4.0->jsonschema!=2.5.0,>=2.4->nbformat==4.2.0) (3.15.0)


.. code:: ipython3

    import yfinance as yf
    import pandas as pd
    import requests
    from bs4 import BeautifulSoup
    import plotly.graph_objects as go
    from plotly.subplots import make_subplots

.. code:: ipython3

    tesla=yf.Ticker("TSLA")

.. code:: ipython3

    tesla_data=tesla.history(period="max")

.. code:: ipython3

    tesla_data.head()




.. raw:: html

    <div>
    <style scoped>
        .dataframe tbody tr th:only-of-type {
            vertical-align: middle;
        }
    
        .dataframe tbody tr th {
            vertical-align: top;
        }
    
        .dataframe thead th {
            text-align: right;
        }
    </style>
    <table border="1" class="dataframe">
      <thead>
        <tr style="text-align: right;">
          <th></th>
          <th>Open</th>
          <th>High</th>
          <th>Low</th>
          <th>Close</th>
          <th>Volume</th>
          <th>Dividends</th>
          <th>Stock Splits</th>
        </tr>
        <tr>
          <th>Date</th>
          <th></th>
          <th></th>
          <th></th>
          <th></th>
          <th></th>
          <th></th>
          <th></th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>2010-06-29</th>
          <td>1.266667</td>
          <td>1.666667</td>
          <td>1.169333</td>
          <td>1.592667</td>
          <td>281494500</td>
          <td>0</td>
          <td>0.0</td>
        </tr>
        <tr>
          <th>2010-06-30</th>
          <td>1.719333</td>
          <td>2.028000</td>
          <td>1.553333</td>
          <td>1.588667</td>
          <td>257806500</td>
          <td>0</td>
          <td>0.0</td>
        </tr>
        <tr>
          <th>2010-07-01</th>
          <td>1.666667</td>
          <td>1.728000</td>
          <td>1.351333</td>
          <td>1.464000</td>
          <td>123282000</td>
          <td>0</td>
          <td>0.0</td>
        </tr>
        <tr>
          <th>2010-07-02</th>
          <td>1.533333</td>
          <td>1.540000</td>
          <td>1.247333</td>
          <td>1.280000</td>
          <td>77097000</td>
          <td>0</td>
          <td>0.0</td>
        </tr>
        <tr>
          <th>2010-07-06</th>
          <td>1.333333</td>
          <td>1.333333</td>
          <td>1.055333</td>
          <td>1.074000</td>
          <td>103003500</td>
          <td>0</td>
          <td>0.0</td>
        </tr>
      </tbody>
    </table>
    </div>



.. code:: ipython3

    url = "https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/labs/project/revenue.htm"
    
    html_data=requests.get(url).text

.. code:: ipython3

    soup=BeautifulSoup(html_data,'html.parser')

.. code:: ipython3

    tesla_revenue = pd.DataFrame(columns=['Date','Revenue'])
    for row in soup.find('tbody').find_all('tr'):
        col=row.find_all("td")
        date=col[0].text
        revenue=col[1].text
        tesla_revenue=tesla_revenue.append({"Date":date,"Revenue":revenue},ignore_index=True)
        
    tesla_revenue.head()




.. raw:: html

    <div>
    <style scoped>
        .dataframe tbody tr th:only-of-type {
            vertical-align: middle;
        }
    
        .dataframe tbody tr th {
            vertical-align: top;
        }
    
        .dataframe thead th {
            text-align: right;
        }
    </style>
    <table border="1" class="dataframe">
      <thead>
        <tr style="text-align: right;">
          <th></th>
          <th>Date</th>
          <th>Revenue</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>0</th>
          <td>2021</td>
          <td>$53,823</td>
        </tr>
        <tr>
          <th>1</th>
          <td>2020</td>
          <td>$31,536</td>
        </tr>
        <tr>
          <th>2</th>
          <td>2019</td>
          <td>$24,578</td>
        </tr>
        <tr>
          <th>3</th>
          <td>2018</td>
          <td>$21,461</td>
        </tr>
        <tr>
          <th>4</th>
          <td>2017</td>
          <td>$11,759</td>
        </tr>
      </tbody>
    </table>
    </div>



.. code:: ipython3

    tesla_revenue.tail()




.. raw:: html

    <div>
    <style scoped>
        .dataframe tbody tr th:only-of-type {
            vertical-align: middle;
        }
    
        .dataframe tbody tr th {
            vertical-align: top;
        }
    
        .dataframe thead th {
            text-align: right;
        }
    </style>
    <table border="1" class="dataframe">
      <thead>
        <tr style="text-align: right;">
          <th></th>
          <th>Date</th>
          <th>Revenue</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>8</th>
          <td>2013</td>
          <td>$2,013</td>
        </tr>
        <tr>
          <th>9</th>
          <td>2012</td>
          <td>$413</td>
        </tr>
        <tr>
          <th>10</th>
          <td>2011</td>
          <td>$204</td>
        </tr>
        <tr>
          <th>11</th>
          <td>2010</td>
          <td>$117</td>
        </tr>
        <tr>
          <th>12</th>
          <td>2009</td>
          <td>$112</td>
        </tr>
      </tbody>
    </table>
    </div>



.. code:: ipython3

    gamestop=yf.Ticker("GME")

.. code:: ipython3

    gme_data=gamestop.history(period="max")

.. code:: ipython3

    gme_data.reset_index(inplace=True)

.. code:: ipython3

    gme_data.head()




.. raw:: html

    <div>
    <style scoped>
        .dataframe tbody tr th:only-of-type {
            vertical-align: middle;
        }
    
        .dataframe tbody tr th {
            vertical-align: top;
        }
    
        .dataframe thead th {
            text-align: right;
        }
    </style>
    <table border="1" class="dataframe">
      <thead>
        <tr style="text-align: right;">
          <th></th>
          <th>Date</th>
          <th>Open</th>
          <th>High</th>
          <th>Low</th>
          <th>Close</th>
          <th>Volume</th>
          <th>Dividends</th>
          <th>Stock Splits</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>0</th>
          <td>2002-02-13</td>
          <td>1.620129</td>
          <td>1.693350</td>
          <td>1.603296</td>
          <td>1.691667</td>
          <td>76216000</td>
          <td>0.0</td>
          <td>0.0</td>
        </tr>
        <tr>
          <th>1</th>
          <td>2002-02-14</td>
          <td>1.712707</td>
          <td>1.716074</td>
          <td>1.670626</td>
          <td>1.683250</td>
          <td>11021600</td>
          <td>0.0</td>
          <td>0.0</td>
        </tr>
        <tr>
          <th>2</th>
          <td>2002-02-15</td>
          <td>1.683250</td>
          <td>1.687458</td>
          <td>1.658001</td>
          <td>1.674834</td>
          <td>8389600</td>
          <td>0.0</td>
          <td>0.0</td>
        </tr>
        <tr>
          <th>3</th>
          <td>2002-02-19</td>
          <td>1.666418</td>
          <td>1.666418</td>
          <td>1.578047</td>
          <td>1.607504</td>
          <td>7410400</td>
          <td>0.0</td>
          <td>0.0</td>
        </tr>
        <tr>
          <th>4</th>
          <td>2002-02-20</td>
          <td>1.615920</td>
          <td>1.662210</td>
          <td>1.603296</td>
          <td>1.662210</td>
          <td>6892800</td>
          <td>0.0</td>
          <td>0.0</td>
        </tr>
      </tbody>
    </table>
    </div>



.. code:: ipython3

    url="https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-PY0220EN-SkillsNetwork/labs/project/stock.html"
    
    html_data=requests.get(url).text

.. code:: ipython3

    soup=BeautifulSoup(html_data,'html.parser')

.. code:: ipython3

    gamestop_revenue = pd.DataFrame(columns=['Date','Revenue'])
    for row in soup.find('tbody').find_all('tr'):
        col=row.find_all("td")
        date=col[0].text
        revenue=col[1].text
        gamestop_revenue=gamestop_revenue.append({"Date":date,"Revenue":revenue},ignore_index=True)
        
    gamestop_revenue.head()




.. raw:: html

    <div>
    <style scoped>
        .dataframe tbody tr th:only-of-type {
            vertical-align: middle;
        }
    
        .dataframe tbody tr th {
            vertical-align: top;
        }
    
        .dataframe thead th {
            text-align: right;
        }
    </style>
    <table border="1" class="dataframe">
      <thead>
        <tr style="text-align: right;">
          <th></th>
          <th>Date</th>
          <th>Revenue</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>0</th>
          <td>2020</td>
          <td>$6,466</td>
        </tr>
        <tr>
          <th>1</th>
          <td>2019</td>
          <td>$8,285</td>
        </tr>
        <tr>
          <th>2</th>
          <td>2018</td>
          <td>$8,547</td>
        </tr>
        <tr>
          <th>3</th>
          <td>2017</td>
          <td>$7,965</td>
        </tr>
        <tr>
          <th>4</th>
          <td>2016</td>
          <td>$9,364</td>
        </tr>
      </tbody>
    </table>
    </div>



.. code:: ipython3

    gamestop_revenue.tail()




.. raw:: html

    <div>
    <style scoped>
        .dataframe tbody tr th:only-of-type {
            vertical-align: middle;
        }
    
        .dataframe tbody tr th {
            vertical-align: top;
        }
    
        .dataframe thead th {
            text-align: right;
        }
    </style>
    <table border="1" class="dataframe">
      <thead>
        <tr style="text-align: right;">
          <th></th>
          <th>Date</th>
          <th>Revenue</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>11</th>
          <td>2009</td>
          <td>$8,806</td>
        </tr>
        <tr>
          <th>12</th>
          <td>2008</td>
          <td>$7,094</td>
        </tr>
        <tr>
          <th>13</th>
          <td>2007</td>
          <td>$5,319</td>
        </tr>
        <tr>
          <th>14</th>
          <td>2006</td>
          <td>$3,092</td>
        </tr>
        <tr>
          <th>15</th>
          <td>2005</td>
          <td>$1,843</td>
        </tr>
      </tbody>
    </table>
    </div>



.. code:: ipython3

    def make_graph(stock_data, revenue_data, stock):
        fig = make_subplots(rows=2, cols=1, shared_xaxes=True, subplot_titles=("Historical Share Price", "Historical Revenue"), vertical_spacing = .3)
        stock_data_specific = stock_data[stock_data.Date <= '2021--06-14']
        revenue_data_specific = revenue_data[revenue_data.Date <= '2021-04-30']
        fig.add_trace(go.Scatter(x=pd.to_datetime(stock_data_specific.Date, infer_datetime_format=True), y=stock_data_specific.Close.astype("float"), name="Share Price"), row=1, col=1)
        fig.add_trace(go.Scatter(x=pd.to_datetime(revenue_data_specific.Date, infer_datetime_format=True), y=revenue_data_specific.Revenue.astype("float"), name="Revenue"), row=2, col=1)
        fig.update_xaxes(title_text="Date", row=1, col=1)
        fig.update_xaxes(title_text="Date", row=2, col=1)
        fig.update_yaxes(title_text="Price ($US)", row=1, col=1)
        fig.update_yaxes(title_text="Revenue ($US Millions)", row=2, col=1)
        fig.update_layout(showlegend=False,
        height=900,
        title=stock,
        xaxis_rangeslider_visible=True)
        fig.show()

.. code:: ipython3

    make_graph(tesla_data,tesla_revenue,'tesla')


::


    ---------------------------------------------------------------------------

    AttributeError                            Traceback (most recent call last)

    /tmp/ipykernel_347/1490691258.py in <module>
    ----> 1 make_graph(tesla_data,tesla_revenue,'tesla')
    

    /tmp/ipykernel_347/2068038883.py in make_graph(stock_data, revenue_data, stock)
          1 def make_graph(stock_data, revenue_data, stock):
          2     fig = make_subplots(rows=2, cols=1, shared_xaxes=True, subplot_titles=("Historical Share Price", "Historical Revenue"), vertical_spacing = .3)
    ----> 3     stock_data_specific = stock_data[stock_data.Date <= '2021--06-14']
          4     revenue_data_specific = revenue_data[revenue_data.Date <= '2021-04-30']
          5     fig.add_trace(go.Scatter(x=pd.to_datetime(stock_data_specific.Date, infer_datetime_format=True), y=stock_data_specific.Close.astype("float"), name="Share Price"), row=1, col=1)


    ~/conda/envs/python/lib/python3.7/site-packages/pandas/core/generic.py in __getattr__(self, name)
       5485         ):
       5486             return self[name]
    -> 5487         return object.__getattribute__(self, name)
       5488 
       5489     def __setattr__(self, name: str, value) -> None:


    AttributeError: 'DataFrame' object has no attribute 'Date'


