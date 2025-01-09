# Câu hỏi: Nếu Video lớn thì có những cách nào để nhúng vào HTML của bạn? Cho ví dụ minh họa?

## Trả lời:

### Cách 1: Sử dụng thẻ `<video>`
#### Code:
```html
<html>
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Nhúng Video Lớn</title>
    </head>
    <body>
        <h1 style="color: red;">Nhúng Video Lớn Bằng Thẻ Video</h1>
        <video width="800" height="450" controls>
            <source src="videosource.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </body>
</html>
```

#### Các thuộc tính của thẻ `<video>`:
- **controls**: Hiển thị các điều khiển phát video như nút Play, Pause, thanh tiến trình, âm lượng, v.v.  
  Ví dụ: `<video controls>`
- **autoplay**: Tự động phát video ngay khi trang được tải. Một số trình duyệt yêu cầu thuộc tính `muted` đi kèm để cho phép autoplay.  
  Ví dụ: `<video autoplay muted>`
- **loop**: Lặp lại video liên tục sau khi phát hết.  
  Ví dụ: `<video loop>`
- **muted**: Tắt âm thanh của video mặc định khi bắt đầu phát.  
  Ví dụ: `<video muted>`

---

### Cách 2: Sử dụng dịch vụ lưu trữ, phát video trực tiếp thông qua thẻ `<iframe>` (YouTube, Google Drive, v.v.)
Nếu video lớn, bạn có thể dùng link video có sẵn và nhúng bằng cách sử dụng thẻ `<iframe>`. **Lưu ý**: cần sử dụng URL nhúng (embed URL) thay vì URL thông thường.

#### Code:
##### - Đối với YouTube:
```html
<html>
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Nhúng Video Từ YouTube</title>
    </head>
    <body>
        <h1>Nhúng Video Từ YouTube</h1>
        <iframe width="800" height="450"
            src="https://www.youtube.com/embed/_lIu6T3Bp2I">
        </iframe>
    </body>
</html>
```

##### - Đối với Google Drive:
```html
<html>
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Nhúng Video Google Drive</title>
    </head>
    <body>
        <h1>Nhúng Video Từ Google Drive</h1>
        <iframe src="https://drive.google.com/file/d/1SWRxFkYG1lcr-bUjpbxtDOkGjJgZDkRO/preview"
                width="800" height="450">
        </iframe>
    </body>
</html>
