```python

from selenium import webdriver
from selenium.webdriver.common.keys import Keys

driver = webdriver.Chrome()
driver.get("https://www.google.co.kr/search?q=intel&hl=ko&sxsrf=ALeKk004ECBYXZq1B7km-TSeuZAiCrdhcQ:1613484714334&source=lnms&tbm=nws&sa=X&ved=2ahUKEwjA9v35yu7uAhVIPnAKHV6YBFsQ_AUoAXoECA0QAw&biw=1022&bih=779")
elem = driver.find_element_by_name("q")
elem.clear()
elem.send_keys("Intel")
elem.send_keys(Keys.RETURN)

elem = driver.find_elements_by_css_selector(".Y3v8qd")[0]
print(elem.text)
 
    
driver.close()

# elem = driver.find_element_by_xpath("//div[@class='language-text highlighter-rouge']/pre[@class='highlight']/code")

# assert "Python" in driver.title
# elem = driver.find_element_by_name("q")
# elem.clear()
# elem.send_keys("pycon")
# elem.send_keys(Keys.RETURN)
# assert "No results found." not in driver.page_source
# driver.close()



```


```python
driver = webdriver.Chrome()
driver.get("https://www.google.co.kr/search?q=intel&hl=ko&sxsrf=ALeKk004ECBYXZq1B7km-TSeuZAiCrdhcQ:1613484714334&source=lnms&tbm=nws&sa=X&ved=2ahUKEwjA9v35yu7uAhVIPnAKHV6YBFsQ_AUoAXoECA0QAw&biw=1022&bih=779")
elem = driver.find_element_by_name("q")
elem.clear()
elem.send_keys("Intel")
elem.send_keys(Keys.RETURN)

for i in range(5):

    elem = driver.find_elements_by_css_selector(".Y3v8qd")[i]
    print(elem.text)
    i = elem
    
driver.close()

```

    [테크월드뉴스=이재민 기자] 글로벌 유통기업 마우저 일렉트로닉스가 Intel Agilex(인텔 애질렉스) F-시리즈 FPGA 개발 키트를 공급한다. 이 키트의 ...
    15일(현지시간) 경제 매체 배런스에 따르면 위스콘신주 투자위원회(SWIB)는 미국 대표 반도체 기업 인텔(INTC) 주식을 대량 매도한 반면 제너럴 ...
    반도체 유통업체 마우저일렉트로닉스가 인텔 애질렉스 F-시리즈 프로그래머블반도체(FPGA) 개발도구를 공급한다고 16일 밝혔다. PCI-SIG 호환 ...
    최근 인텔은 범용 메모리에 가까운 3D XPoint 기술을 사용하는 Optane을 발표했습니다. 이것은 주로 RAM으로 작동하기에 충분히 빠른 비 휘발성 ...
    그는 경력의 첫 걸음을 지난 1979년 인텔에서 엔지니어로 시작했고, 이어 최고기술책임자(CTO)까지 역임한 입지전적인 인물이자, 대표적인 '인텔맨' ...
    


```python
driver = webdriver.Chrome()
driver.get("https://www.google.co.kr/search?q=intel&hl=ko&sxsrf=ALeKk004ECBYXZq1B7km-TSeuZAiCrdhcQ:1613484714334&source=lnms&tbm=nws&sa=X&ved=2ahUKEwjA9v35yu7uAhVIPnAKHV6YBFsQ_AUoAXoECA0QAw&biw=1022&bih=779")
elem = driver.find_element_by_name("q")
elem.clear()
elem.send_keys("Intel")
elem.send_keys(Keys.RETURN)

for i in range(5):

    elem = driver.find_elements_by_css_selector(".Y3v8qd")[i]
    print(elem.text)
    i = elem
    
driver.close()

```
