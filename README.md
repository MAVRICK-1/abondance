# Abondance: Python library for Internet Health Report API

### Installation
Get the latest source files:
```
git clone git@github.com:InternetHealthReport/abondance.git
```

Install dependencies and install abondance:
```
cd abondance
sudo pip install -r requirements.txt 
sudo python setup.py install
```
### Example: Retrieve dependencies for AS2501 on September 15th, 2018
```python
from abondance.hegemony import Hegemony

hege = Hegemony(originasns=[2501], start="2018-09-15", end="2018-10-16")

for r in hege.get_results():
  print(r)
```
