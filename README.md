# Zhuhai-rental-house
### execution steps
### github link https://github.com/Chakfung/Zhuhai-rental-house
1. Create virtual environment
   ```sh
   python -m venv venv
   ```

2. activate venv
   ```sh
   ./venv/Script/activate
   ```
   
3. Install libraries    
   ```sh
   pip install -r requirements.txt
   ```
4. run crawler 
   ```sh
   cd zhuhai_crawler
   ```
   Because crawling takes a long time, it is recommended that you use the "output.csv" dataset in the root directory
   ```sh
   scrapy crawl zhuhai -o ../output.csv
   ```
5. data analysis part run analyse.ipynb in the root directory(use venv).
In map visualization part, for api quota limitation just use latitude_longitude.csv directly
6. python simulation part
   use simulation.ipynb
7. web simulation part:
   i have deploy the project on server, you can visit http://8.134.104.62/
    ```sh
    cd simulation
    ```
    Installing front-end packages (dependent)
    ```sh
    yarn install
    ```
    run project
    ```sh
    yarn serve
    ```
    visit website http://localhost:8000/

### python version
Python 3.11.2



    
