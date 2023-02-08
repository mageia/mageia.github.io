# Example

!> 一段重要的内容，可以和其他 **Markdown** 语法混用。


## Tag Example
<!-- tabs:start -->
#### **Python**
```python
import requests
requests.get('https://www.baidu.com')
```

#### **Java**
```java
package com.ushareit.model.meta;
```

#### **Golang**
```go
package main
```
<!-- tabs:end -->


## Mermaid Example

### Mermain graph

```mermaid
graph LR
emperor((朱八八))-.子.->朱五四-.子.->朱四九-.子.->朱百六


朱雄英--长子-->朱标--长子-->emperor
emperor2((朱允炆))--次子-->朱标
朱樉--次子-->emperor
朱棡--三子-->emperor
emperor3((朱棣))--四子-->emperor
emperor4((朱高炽))--长子-->emperor3
```

### Mermain sequenceDiagram

```mermaid
sequenceDiagram
	par 第一次握手
		alt Client Hello
		Client->>Server: ClientRandom, TLSVersion, Cipher
		end
	end

	par 第二次握手
		rect rgb(147, 188, 193)
      alt Server Hello
      Server-->>Client: ServerRandom, TLSVersion, Cipher, ServerCertificate
      end
		end
	end

	par 第三次握手
		alt Client Key Exchange
		Client->>Server: pre_master_key
		end
		alt Change Cipher Spec
		Client->>Server: 
		end
		alt Enceypt Handshake Message
		Client->>Server: 摘要，Finish报文
		end
	end

	par 第四次握手
    rect rgb(147, 188, 193)
      alt Change Cipher Spec
      Server-->>Client: 
      end
      alt Enceypt Handshake Message
      Server-->>Client: 摘要，Finish报文
      end
    end
	end
```
