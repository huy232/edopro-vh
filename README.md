## Edopro Việt Hóa Thẻ Bài

Vào thư mục game EDOPro của bạn.

> Ví dụ: `C:\ProjectIgnis\config\user_configs.json`. 

Mở file *user_configs.json* bằng **Notepad** hoặc bất kỳ trình đọc nào, áp dụng:

```json
{
  "repos": [
    <!-- Các gói repo khác  -->
    		{
          "url": "https://github.com/huy232/edopro-vh",
          "repo_name": "EDOPro Tiếng Việt",
          "repo_path": "./config/languages/Tiếng Việt",
          "is_language": true,
          "data_path": "",
          "language": "",
          "should_update": true,
          "should_read": true
        }
    <!-- Các gói repo khác -->
  ],
  "urls" : [
    <!-- Các URL khác của bạn -->
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

> [!CAUTION]
> Nếu có những lá mới hơn chưa được dịch sẽ tự fallback những lá đó về Tiếng Anh hoặc ngôn ngữ phù hợp.

> [!IMPORTANT]
> Những nguồn cho Repo này.

* Mình sử dụng và modify file *`string.conf`* từ nguồn này:
  - [ Repo Edopro-Card-Vietsub của TriDungSongToan](https://github.com/TriDungSongToan/Edopro-Card-VietSub)

* Những thẻ bài việt hóa chủ yếu đến từ API:
  - [YGO Việt Nam](https://ygovietnam.com/)

* Việt hóa hiệu ứng của những lá bài:
  - Chủ yếu mình tự dịch

