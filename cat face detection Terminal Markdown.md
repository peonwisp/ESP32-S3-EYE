要在windowns系統下使用ESP-IDF tool需要先去下載檔案，網址 : https://dl.espressif.com/dl/esp-idf/

開啟ESP-IDF 5.2 PowerShell 或 ESP-IDF 5.2 CMD

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/ac03cf2d-bdd8-4ef5-9d80-21d0a5b46785)

開啟exe後，路徑會顯示下安裝所存放的地方 C:\Espressif\frameworks\esp-idf-v5.2.1>

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/e7566bf1-580e-4299-af95-dda1c99ebf3b)

安裝esptool，指令 :  pip install esptool

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/34e4e871-eef8-429e-a989-b0200acc9a6a)

安裝ninja，指令 :  pip install ninja

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/72816451-be36-4613-90be-cb0965949ffa)

安裝cmake，指令 :  pip install cmake

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/530420e9-fa21-4d87-b67c-5518829d4c9b)

創建一個任意名稱的資料夾，舉例: 名稱為esp的資料夾，指令 : mdkir esp

切換到名為 esp 的目錄，指令 : cd esp 

當前路徑顯示為 C:\Espressif\frameworks\esp-idf-v5.2.1\esp>

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/709917f5-6447-476c-b54b-9f84df8c8dad)

輸入遞歸克隆 esp-who 專案的 Git 儲存庫，指令 : git clone --recursive https://github.com/espressif/esp-who.git

輸入遞歸克隆 esp-idf 專案的 Git 儲存庫，指令 : git clone --recursive https://github.com/espressif/esp-idf.git

於CMD輸入ls可以當到當前目錄下所有資料

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/c0888ba4-953d-4339-b990-ed838ac86214)

切換到名為 esp-idf 的目錄，指令 : cd esp-idf

當前路徑顯示為 C:\Espressif\frameworks\esp-idf-v5.2.1\esp\esp-idf>

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/88dd4299-151d-4675-a7d9-aed7dfdd038e)

執行 install.bat 腳本，安裝開發環境，指令 : install.bat

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/d53de752-f8e5-4e9a-b8dc-b714dfeab48e)

執行完install.bat後，顯示出All done! You can now run:export.bat，表示install.bat已有執行完成，可以執行export.bat

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/20268d16-fe05-4859-88c1-8b49b33758df)

執行 export.bat 腳本，設置環境變量，指令 : export.bat

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/9033126e-01d2-40ee-ba71-fd4e9b067325)

執行完export.bat後，顯示出Go to the project directory and run:idf.py build，表示export.bat已有執行完成，可以執行idf.py build

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/2d6d9c1e-7a82-4fea-9226-9ee4bc93cce5)

以cat_face_detection_terminal為範例

切換到上一層路徑，指令 : cd ..

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/2c1b926d-7761-4c00-a316-af41d19d3300)

當前路徑顯示為 C:\Espressif\frameworks\esp-idf-v5.2.1\esp>

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/0b1ba92b-c056-4c2d-8285-7c4bf6ec3d60)

切換到名為 esp-who 的目錄，指令 : cd esp-who

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/3ab57684-feed-4e4d-86c6-a83b5d890233)

當前路徑顯示為 C:\Espressif\frameworks\esp-idf-v5.2.1\esp\esp-who>

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/fb64456d-e86b-420a-8323-5c7af894e40a)

切換到esp-who底下名為 examples 的目錄，指令 : cd examples

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/14d0487a-4796-42cd-8b36-380221944f22)

當前路徑顯示為 C:\Espressif\frameworks\esp-idf-v5.2.1\esp\esp-who\examples>

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/75040780-e6c8-4b94-9d91-7154056cedf2)

examples資料夾內有很多範例，這邊選擇cat_face_detection做說明

切換到examples底下名為 cat_face_detection 的目錄，指令 : cd cat_face_detection

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/a4532382-13cd-417a-8a3f-6fb896ddc384)

當前路徑顯示為 C:\Espressif\frameworks\esp-idf-v5.2.1\esp\esp-who\examples\cat_face_detection>

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/5a955070-00f8-4234-b83d-4315e8143efc)

cat_face_detection資料夾內有lcd、terminal、web三個程式碼可用，這邊選擇terminal做說明

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/cef70842-3275-40c1-b9c5-9289c5cb8163)

切換到cat_face_detection底下名為 terminal 的目錄，指令 : cd terminal

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/e0e3a8c1-246c-4073-b750-a6ca943f1dbd)

當前路徑顯示為 C:\Espressif\frameworks\esp-idf-v5.2.1\esp\esp-who\examples\cat_face_detection\terminal>

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/ceebc668-7489-4377-97ff-d5dd59ec17a0)

執行設定目標芯片，指令 : idf.py set-target esp32s3

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/e2e68ccf-7bc7-47d1-ab4b-4bfee82eba01)

執行編譯指令，指令 : idf.py fullclean

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/0ee79c8c-e947-4164-a428-38493a3a6a0c)

執行建立專案指令，指令 : idf.py build

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/426c1638-4f46-4401-ab80-a4103a3b8cfe)

此時build完的檔案會出現在資料夾中

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/715bb563-2358-494a-a97f-a95de43c30db)

專案建立完後，需要做清除，指令 : idf.py flash

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/2d2cb6d1-872c-4b08-a4b3-08d93610756f)

燒錄會使用到build資料夾底下的bootloader.bin與patition.bin和cat_face_detection_terminal.pin，共三個檔案

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/abb1ec58-b579-4ec7-bada-2f4562cad359)

預設的bootloader.bin在build資料夾底下的bootloader資料夾，patition.bin在patition資料夾底下的bootloader資料夾，cat_face_detection_terminal.pin則在build資料夾下

開始燒錄需要注意三個bin檔的位置，如有更動bin檔，燒錄的指令需要做更動，這邊以預設好的路徑做燒錄 (console Baud rate 設定任何數字都可以，以115200做說明)

開始燒錄cat_face_detection_terminal，指令 : esptool.py -p COM3 -b 115200 --before default_reset --after hard_reset --chip esp32s3 write_flash --flash_mode dio --flash_size 8MB --flash_freq 
80m 0x0 build\bootloader\bootloader.bin 0x8000 build\partition_table\partition-table.bin 0x10000 build\cat_face_detection_terminal.bin

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/bfd52127-7ead-43d9-9ae0-0488d82c3660)

最後燒錄完成後，可從CMD看到最後一行字為 Hard resetting via RTS pin...

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/1cd8ffa1-09d4-408b-a7d1-c793577b0337)

使用putty 或 MobaXterm 來看輸出結果

![image](https://github.com/peonwisp/ESP32-S3-EYE/assets/155973617/1b23d477-b53e-4c27-8227-8c203a8773fc)
