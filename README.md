## Edopro Việt Hóa Thẻ Bài

Vào thư mục game EDOPro của bạn.

> Ví dụ: `C:\ProjectIgnis\config\user_configs.json`. 

Mở file *user_configs.json* bằng **Notepad** hoặc bất kỳ trình đọc nào, áp dụng:

```json
{
  "repos": [
     {
      "__comment": "Gói repo khác của bạn",
      "url": "URL",
      "repo_name": "REPO NAME",
      "repo_path": "REPO PATH",
    },
    {
      "__comment": "EDOPro Tiếng Việt",
      "url": "https://github.com/huy232/edopro-vh",
      "repo_name": "EDOPro Tiếng Việt",
      "repo_path": "./config/languages/Tiếng Việt",
      "is_language": true,
      "data_path": "",
      "language": "",
      "should_update": true,
      "should_read": true
    },
    {
      "__comment": "Gói repo khác của bạn",
      "url": "URL",
      "repo_name": "REPO NAME",
      "repo_path": "REPO PATH",
    }
  ],
  "urls" : [
  ] 
}
```

Sau đó, vào game.
Trước tiên bạn hãy kiểm tra xem việc cài đặt tiếng Việt đã thành công chưa bằng việc:

<img src="https://i.imgur.com/xIq8rGr.png" alt="Check install" width="480px" height="auto">

Nếu đã thành công, hãy mở Menu lên và thay đổi sang ngôn ngữ Tiếng Việt

<img src="https://i.imgur.com/qjgHzC2.png" alt="Check install 2" width="480px" height="auto">


Game sẽ tự động việt hóa những lá bài hiện có.

Tiến độ hiện tại:

- ✅ Những lá bài Official TCG-OCG: 13727 lá bài
- ✅ Những lá bài GOAT Format: 1799 lá bài
- ✅ Những lá bài EDISON Format: 3839 lá bài
- ✅ Những lá bài Rush Duel: 2684 lá bài
- ✅ Update tạm thời hơn 60 Pre-Errata Card
- ✅ Cards.delta
- ✅ Pre-release
- ✅ Re-release 
- 🔳 -----------------------------------

> [!CAUTION]
> Nếu có những lá mới hơn chưa được dịch sẽ tự fallback những lá đó về Tiếng Anh hoặc ngôn ngữ phù hợp.

> [!IMPORTANT]
> Những nguồn cho Repo này.

* Mình sử dụng và modify file *`string.conf`* từ nguồn này:
  - [ Repo Edopro-Card-Vietsub của TriDungSongToan](https://github.com/TriDungSongToan/Edopro-Card-VietSub)

* Những thẻ bài việt hóa chủ yếu đến từ API:
  - [YGO Việt Nam](https://ygovietnam.com/)

* Việt hóa hiệu ứng của những lá bài:
  - Chủ yếu mình tự dịch/sửa + AI Translate


> [!NOTE] 
> File user_configs.json của mình, chia sẻ nếu các bạn muốn có ảnh HD Upscale + Ban list, card pool của các format khác + Việt Hóa + Skin Pack

Những URLs (không phải URLs bên trong `repos`) dưới chỉ áp dụng nếu bạn chưa có những lá bài HD hoặc tương tự như vậy bên trong thư mục `pics` ở ProjectIgnis/pics. 

Ví dụ: Bạn chưa có lá bài HD Blue-Eyes White Dragon 

=> Một trong những URL bên dưới sẽ tìm và tải về cho bạn 1 lá bài HD (Hoặc Việt Hóa lá bài hoàn toàn nếu bạn để nó ở thứ tự đầu tiên) 

=> Sau đó sẽ áp dụng 1 trong những URL bên dưới để tải lá bài đó về và sẽ sao lưu nó ở bên trong thư mục pics của EDOPro. Những lần sau những lá bài này sẽ không dùng những URL bên dưới nữa mà sẽ dùng ở bên trong folder pics ở trong máy hoặc điện thoại của bạn để giảm băng thông cho server tải ảnh 

=> Hãy cân nhắc bạn muốn sử dụng thứ tự nào nếu bạn chưa có hoặc chưa tải bất kỳ gói HD Card nào (có thể kiểm tra thư mục pics và bạn sẽ biết bạn hiện có những lá bài nào, chúng sẽ theo dạng `ID.jpg`, VD: `56889.jpg`, `220414.jpg`, ...). Nếu đã có rồi nhưng vẫn muốn thử, hãy backup folder pics ở đâu đó phòng trường hợp những lá bài mới tải về không được như ý bạn, như vậy chỉ việc chép đè lại thư mục pics và bạn sẽ không cần áp dụng những URL dưới đây nữa cho những thẻ đã có rồi.

* Việc này rất tốt cho tương lai, nếu một trong những server thuộc URL dưới đây có thẻ HD mới cập nhật, và trong folder pics của bạn chưa có, khi tìm tới những lá bài này trong EDOPro. Chúng sẽ tự tải về thẻ HD cho bạn.

File `user_configs.json` hoàn chỉnh của mình:

```
{
  "repos": [
    {
      "__comment": "EDOPro Tiếng Việt",
      "url": "https://github.com/huy232/edopro-vh",
      "repo_name": "EDOPro Tiếng Việt",
      "repo_path": "./config/languages/Tiếng Việt",
      "is_language": true,
      "data_path": "",
      "language": "",
      "should_update": true,
      "should_read": true
    },
    {
      "__comment": "EDOPro Skinpack",
      "url": "https://github.com/Lahrenheit/EDOPRO-Skinpack",
      "repo_name": "Lahrenheit EDOPro Skinpack",
      "repo_path": "./skin/",
      "should_update": true,
      "should_read": true
    },
    {
      "__comment": "Rush Duel gói HD Card",
      "url": "https://github.com/Yoshi80/Rush-HD-Pictures",
      "repo_name": "Rush Duel HD Card Project",
      "repo_path": "./repositories/rush-hd",
      "has_core": false,
      "data_path": "",
      "script_path": "script",
      "pics_path": "pics",
      "expansions_path": "expansions",
      "should_update": true,
      "should_read": true
    },
    {
      "__comment": "Các Ban list - Card pool cho các Format khác như (Edison, JPLT, etc.)",
      "url": "https://github.com/termitaklk/lflist",
      "repo_name": "Forbidden & Limited Card Lists of other FORMAT",
      "repo_path": "./repositories/lflists-other",
      "lflist_path": ".",
      "should_update": true,
      "should_read": true
    },
    {
      "url": "https://github.com/TamamoNoMae13/ocg-ae-banlist-for-edopro",
      "repo_name": "OCG AE Banlist for EDOPro",
      "repo_path": "./repositories/ocg-ae-banlist",
      "lflist_path": ".",
      "should_update": true,
      "should_read": true
    }
  ],
  "urls": [
    {
      "__comment": "Ảnh HD AI upscale, thứ tự 1",
      "url": "https://raw.githubusercontent.com/TheBv/Yugioh-Cards/master/esrgan-2x/{}.jpg",
      "type": "pic"
    },
    {
      "__comment": "Ảnh HD từ YGOProdeck, thứ tự 2",
      "url": "https://images.ygoprodeck.com/images/cards/{}.jpg",
      "type": "pic"
    },
    {
      "__comment": "Ảnh HD từ Formatlibrary, thứ tự 3",
      "url": "https://cdn.formatlibrary.com/images/cards/{}.jpg",
      "type": "pic"
    },
    {
      "__comment": "Ảnh HD từ YGO Việt Nam, thứ tự 4",
      "url": "https://ygovietnamcdn.azureedge.net/storage/Card/{}.jpg",
      "type": "pic"
    },
    {
      "url": "https://ygovietnam.blob.core.windows.net/storage/Card/{}.jpg",
      "type": "pic"
    },
    {
      "__comment": "Ảnh được việt hóa (tên bài + nội dung), thứ tự 5, nếu bạn muốn lá bài Việt Hóa từ bên YGO Việt Nam, bạn có thể đẩy thứ tự này lên thành thứ tự 1 và sắp xếp các thứ tự khác xuống thấp hơn.",
      "url": "https://ygovietnamcdn.azureedge.net/storage/CardVietSub/{}.jpg",
      "type": "pic"
    },
    {
      "__comment": "Ảnh HD Bài Môi Trường cho Rush, thứ tự riêng, vì đây là ảnh Môi Trường cho Rush, không liên quan đến bên trên",
      "url": "https://raw.githubusercontent.com/Yoshi80/Rush-HD-Pictures/master/pics/field/{}.png",
      "type": "field"
    }
  ],
  "servers": [],
  "posixPathExtension": "/usr/local/bin:/Library/Frameworks/Mono.framework/Versions/Current/Commands"
}
```
