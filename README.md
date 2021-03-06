# Struts2-048
CVE-2017-9791 Struts2 RCE 취약점

요약 : Struts2 3.x 버전에서 Struts1 plugin을 사용한 어플리케이션 존재 시 취약

지난 번 발생했던 cve-2017-5638 취약점은 Struts2를 사용하는 경우, 존재하지 않는 페이지에도 취약점이 발생했던 것과는 달리 이번 cve-2017-9791에서는 Struts2 기반에서 Struts1 plugin을 사용하는 경우에만 유효합니다.

참고 URL : https://cwiki.apache.org/confluence/display/WW/S2-048
 2.3.x 버전을 사용하고 있는 경우 지난 번과 이번에 발생된 취약점으로 인하여 전 버전이 취약한 상황입니다.
 - 2.3.31 및 하위 버전 -> CVE-2017-5638 취약 
 - 2.3.32 및 하위 버전에서 struts1 plugin 사용 시 취약 -> CVE-2017-9791 취약

조치방안 : Apache Struts 2.5.10.1 이상 버전으로 업데이트

Author: DragonEgg
```python
def Usage():
    print 'check:'
    print '    python file.py http://1.1.1.1/struts2-showcase/integration/saveGangster.action'
    print 'poc:'
    print '    python file.py http://1.1.1.1/struts2-showcase/integration/saveGangster.action command'
```

# Demo
![image](https://github.com/dragoneeg/Struts2-048/blob/master/demo.jpg)
