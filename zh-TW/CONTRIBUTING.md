<p align="center">
    <a href="https://doc.anytype.io">
        <img src="../.gitbook/assets/anytype-logo-360px.png" alt="Docs-Logo" width="100px" height="100px">
    </a>
</p>


## 目錄

- [**介紹**](#Intro)
- [**貢獻流程**](#contribution-process)
- [**檔案結構**](#file-structure)
- [**慣例**](#conventions)
  - [**文字格式**](#text-formats)
  - [**列表**](#lists)
  - [**區塊**](#blocks)
  - [**媒體**](#media)

## 介紹

ℹ️ 請所有使用者在貢獻到文檔前閱讀 [Code of Conduct](https://github.com/anytypeio/community/blob/main/README.md#code-of-conduct) 和 [Gitbook Conventions](#conventions)。歡迎您提出任何Pull Request(下稱PR)中的修改建議，並參與 [改良doc.anytype.io](https://community.anytype.io/t/improvements-for-doc-anytype-io/2862) 中的討論. 請參照以下步驟貢獻. 如果您對 _git_ 和 _GitHub_ 不熟悉，我們建議您參考 [GitHub指南](https://guides.github.com/introduction/flow/). 


## 貢獻流程

1. 分叉(Fork)此儲存庫
2. (可選) 克隆(Clone)此分叉
   - 使用 SSH
     ```shell
     git clone --filter=tree:0 git@github.com:anytypeio/community.git
     ```
   - 使用 HTTPS
     ```shell
     git clone --filter=tree:0 https://github.com/anytypeio/community.git
     ```
   - 使用 GitHub CLI
     ```shell
     gh repo clone anytypeio/community -- --filter=tree:0
     ```
3. 從最新的 `main` 建立新分支(Branch)
4. 在新的分支上做出修改
5. 提交(Commit)並推送(Push)到新的分支
6. 建立新的PR
7. 將 [Vladimir](https://github.com/d1eselboy), [Divyanshu](https://github.com/div3xi) 或 [Enda](https://github.com/endac) 指定為PR審核員。

## 檔案結構

* 添加或刪除文檔中的任何頁面都需要將其添加到 [SUMMARY.md](https://github.com/anytypeio/docs/blob/main/SUMMARY.md) 的**目錄**中
  * 使用縮排表示頁面的嵌套
  * 使用Markdown URL進行頁面連結，例如：
    ```
    [Navigation](https://github.com/anytypeio/docs/blob/main/features/navigation.md)
    ```
* 所有文件保存為 **Markdown.md**
* 對於嵌套的頁面，它們需要放置在分類資料夾中。如果不存在則可以創建該文件夾
* 要使用圖像，它們必須全部放在 [.gitbook/assets](https://github.com/anytypeio/docs/tree/main/.gitbook/assets) 資料夾中並從該資料夾中引用 
    > 所以媒體都應該處於淺色模式
## 慣例

> 這些是Gitbook自Markdown創建文檔時遵循的規則。在進行任何更改時請遵循這些規則。


### 文字格式

- # 標題 1
  ```
  # 標題 1
  ```
  
- ## 標題 2
  ```
  ## 標題 2
  ```
  
- ### 標題 3
  ```
  ### 標題 3
  ```
  
- **粗體**
  ```
  **粗體**
  ```
  
- _斜體_
  ```
  _斜體_
  ```
  
- ~~刪除線~~
  ```
  ~刪除線~
  ```
  
- 水平線
  ```
  ---
  ```
  
- [連結](#)
  ```
  [連結名稱](https://example.com)
  ```

- ![圖片](#)
  ```
  ![圖片](http://url/a.png)
  ```

- `行內程式碼`
  ```
  `行內程式碼`
  ```

### 列表

- **無序列表**
  ```
  * 項目 1
  * 項目 2
  * 項目 3
      或
  - 項目 1
  - 項目 2
  - 項目 3
  ```

- **有序列表**
  ```
  1. 項目 1
  2. 項目 2
  3. 項目 3
  ```

- **任務列表**
  ```
  * [ ] 未勾選任務
  * [x] 勾選任務
  ```
  
### 區塊

- **程式碼區塊**
```
``` 建立新程式碼區塊。
```py 創建一個帶有Python語法突出顯示的新程式碼區塊。
```

- **引用**
  ```
  使用 > 開始引用區塊.
  ```

- **訊息提示區塊**
  ```
  {% hint style="info" %} 訊息提示區塊 {% endhint %}
  ```
  <p align="left">
    <a href="https://doc.anytype.io">
        <img src="https://raw.githubusercontent.com/anytypeio/community/main/assets/info-hints-block.png" alt="info-hints">
    </a>
  </p>
  
- **警告提示區塊**
  ```
  {% hint style="warning" %} 警告提示區塊 {% endhint %}
  ```
    <p align="left">
    <a href="https://doc.anytype.io">
        <img src="https://raw.githubusercontent.com/anytypeio/community/main/assets/warning-hints-block.png" alt="warning-hints">
    </a>
  </p>
  
- **成功提示區塊**
  ```
  {% hint style="success" %} 成功提示區塊 {% endhint %}
  ```
    <p align="left">
    <a href="https://doc.anytype.io">
        <img src="https://raw.githubusercontent.com/anytypeio/community/main/assets/success-hints-block.png" alt="success-hints">
    </a>
  </p>
  
- **危險提示區塊**
  ```
  {% hint style="danger" %} 危險提示區塊 {% endhint %}
  ```
    <p align="left">
    <a href="https://doc.anytype.io">
        <img src="https://raw.githubusercontent.com/anytypeio/community/main/assets/danger-hint-block.png" alt="danger-hints">
    </a>
  </p>

### 媒體

- **區塊:** 創建媒體區塊時，需要使用以下慣例
  ```
  ![媒體標題](<.gitbook/assets/file-name>)
  
  E.g.:
  
  ![首頁](<.gitbook/assets/Screenshot 2021-11-05 at 18.45.31.png>)
  ```
  添加媒體區塊時，如果您添加的頁面是嵌套的，請適當使用 `../` 來使嵌入工作。

- **檔案儲存 :** 任何媒體必須首先上傳到 [.gitbook/assets/](https://github.com/anytypeio/docs/tree/main/.gitbook/assets) 資料夾。之後才能在文件中使用。您可能會看到 GitBook 在現有頁面中嵌入專有格式 `{% embed url="`，您不需要使用它。

- **檔案格式:** 這些是唯一可以接受上傳到文件中的媒體檔案格式。
    - **影片:**
    
      > ✔️ 僅使用 **MP4**  
      > ❌ 禁止使用 **gifs** 或其他格式
      
    - **圖片:**
      
      > ✔️ 僅使用 **PNG** 和 **JPG** 圖片  
      > ❌ 禁止其他格式

- **大小限制:**  每個媒體文件上傳的大小限制為 5 MB。1000px 寬的圖片和影片就非常清晰了，但可以將 4K 文件大小減少 75%。

- **命名:** 為減少混淆，上傳時請以人類可讀格式重新命名您的檔案
  ```
  <圖片標題>-<頁面>.<文件格式>

  例如：
  ✔️ loadingscreen-intro.png
  ❌ Screenshot 2021-11-05 at 18.45.31.png
