## Edopro Việt Hóa Thẻ Bài

Vào thư mục game EDOPro của bạn.

> Ví dụ: `C:\ProjectIgnis\config\user_configs.json`. 

Mở file *user_configs.json* bằng **Notepad** hoặc bất kỳ trình đọc nào, áp dụng:

```json
{
  "repos": [
    {
    <!-- Các gói repo khác  -->

		"url": "https://github.com/huy232/edopro-vh",
		"repo_name": "EDOPro Vietnamese Localization",
		"repo_path": "./repositories/edopro-vh",
		"should_update": true,
		"should_read": true
	    
    <!-- Các gói repo khác -->
    }
  ],
  "urls" : [
    <!-- Các URL khác của bạn -->
  ] 
}
```

Sau đó, vào game, sẽ tự động việt hóa những lá bài hiện có.

> [!CAUTION]
> Nếu có những lá mới hơn chưa được dịch sẽ tự fallback những lá đó về Tiếng Anh hoặc ngôn ngữ phù hợp.

> [!IMPORTANT]
> Những nguồn cho Repo này.

Mình sử dụng, modify file `string.conf` từ nguồn này:
- [Repo Edopro-Card-Vietsub của TriDungSongToan](https://github.com/TriDungSongToan/Edopro-Card-VietSub)

Những thẻ bài việt hóa chủ yếu đến từ API:
- [YGO Việt Nam](https://ygovietnam.com/)

Việt hóa hiệu ứng của những lá bài:
- Chủ yếu mình tự dịch

