1\. **e\_lfanew:** 0xF0

2. **COFF header:**

&#x09;Machine: 0x014C

&#x09;NumberOfSections: 0x0005

&#x09;TimeDateStamp: 0x6AD21529

3\. **Optional header:**

&#x09;Magic: 0x010B

&#x09;AdressOfEntryPoint: 0x125A

&#x09;ImageBase: 0x00400000

4\. **Tabela de sectiuni:**

&#x09;Name: 2E 74 65 78 74 00 00 00

&#x09;VirtualAddress:   0x1000

&#x09;PointerToRawData: 0x400

5\. **FileOffset** = AddressOfEntryPoint - VirtualAddress + PointerToRawData = 0x65A

&#x20;  **VA** = ImageBase + AddressOfEntryPoint = 0x40125A

6\.

Primii bytes la 0x65A: E8 A5 02 00 00

E8 = call -> call \_\_security\_init\_cookie



urmat de un E9 71 FE FF FF (jmp) la 0x65F

Compilator: MSVC.

Alt hint: Rich header.

