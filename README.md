# geetest-slider-captcha-bypass
![](https://img.shields.io/badge/Python-Selenium-blue) ![](https://img.shields.io/badge/Python-OpenCV-yellow)


Bypass Geetest Slider Captcha using _**Selenium and OpenCV**_

<hr>
To install required dependencies, run this in a shell/terminal

```
pip install -r requirements.txt
apt install chromium-chromedriver # if running of linux
```
Now import the `GSC_solver` class
```
from gsc import GSC_solver

gcs = GSC_solver()
search_term = 'bts_official_bighit'
driver = gcs.solve(f'https://www.tiktok.com/@{search_term}')
```
or
```
. . .

driver = webdriver.Chrome(chrome_driver_path, desired_capabilities=caps, options=chrome_options)
search_term = 'bts_official_bighit'
driver.get(f'https://www.tiktok.com/@{search_term}')

# Solve captcha by passing webdriver object
driver = gcs.solve(driver)

. . .
```
<hr>
<p>
<img src="snapshot/0b8796d53da6cd73610cb336e2cc45da/captcha.gif" width="300" height="250" />
<img src="snapshot/0c2e924a9af52a7a17b90dd7dd2651ad/captcha.gif" width="300" height="250" />
<img src="snapshot/0c3222c9aa061ca1bac3d0af4e440866/captcha.gif" width="300" height="250" />
<p>
<p>
<img src="snapshot/0c84a2a6410b81ed57add4c33075f5c9/captcha.gif" width="300" height="250" />
<img src="snapshot/0ca8cb7f7a01bfbf40ce2dc4ef8fcbb3/captcha.gif" width="300" height="250" />
<img src="snapshot/0cfbc78517fffb094c0f2a0c3b2fc3b7/captcha.gif" width="300" height="250" />
<p>
<p>
<img src="snapshot/0d1e34ef2624d8f3f0da8095e1c8dc00/captcha.gif" width="300" height="250" />
<img src="snapshot/0db50c4cc2b9048111447d80417ee47f/captcha.gif" width="300" height="250" />
<img src="snapshot/0de3867dafbb6744b68bc883a5027cc7/captcha.gif" width="300" height="250" />
<p>
<hr>
<p>
<img src="snapshot/0b8796d53da6cd73610cb336e2cc45da/process.gif" width="300" height="250" />
<img src="snapshot/0c2e924a9af52a7a17b90dd7dd2651ad/process.gif" width="300" height="250" />
<img src="snapshot/0c3222c9aa061ca1bac3d0af4e440866/process.gif" width="300" height="250" />
<p>
<p>
<img src="snapshot/0c84a2a6410b81ed57add4c33075f5c9/process.gif" width="300" height="250" />
<img src="snapshot/0ca8cb7f7a01bfbf40ce2dc4ef8fcbb3/process.gif" width="300" height="250" />
<img src="snapshot/0cfbc78517fffb094c0f2a0c3b2fc3b7/process.gif" width="300" height="250" />
<p>
<p>
<img src="snapshot/0d1e34ef2624d8f3f0da8095e1c8dc00/process.gif" width="300" height="250" />
<img src="snapshot/0db50c4cc2b9048111447d80417ee47f/process.gif" width="300" height="250" />
<img src="snapshot/0de3867dafbb6744b68bc883a5027cc7/process.gif" width="300" height="250" />
<p>
<hr>
If you want to save snapshots like these, give location at `snapshot_path` in `solve`
```
gcs.solve(. . . , snapshot_path = 'enter_path_here')
```
