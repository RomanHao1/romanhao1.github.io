# 作品集网站使用指南

## 项目结构
```
CODE/
├── index.html          # 网站主页面
├── style.css           # 网站样式文件
├── images/             # 图片资源文件夹
│   └── profile.jpg     # 个人照片（示例文件名）
│   └── work1.jpg       # 作品图片1（示例文件名）
│   └── work2.jpg       # 作品图片2（示例文件名）
│   └── work3.jpg       # 作品图片3（示例文件名）
│   └── work4.jpg       # 作品图片4（示例文件名）
└── videos/             # 视频资源文件夹
    └── video1.mp4      # 视频作品1（示例文件名）
    └── video2.mp4      # 视频作品2（示例文件名）
```

## 如何添加图片作品

1. 将您的图片作品复制到 `images` 文件夹中
2. 在 `index.html` 文件中找到对应的图片标签（搜索 `images/work1.jpg` 等示例路径）
3. 将 `src` 属性的值修改为您的图片文件名，例如：
   ```html
   <img src="images/your-image-filename.jpg" alt="作品标题">
   ```
4. 同时更新 `alt` 属性的值，提供作品的简要描述
5. 可以修改作品的标题和描述：
   ```html
   <div class="portfolio-overlay">
       <h3>您的作品标题</h3>
       <p>您的作品描述</p>
   </div>
   ```

## 如何添加视频作品

1. 将您的视频作品复制到 `videos` 文件夹中
2. 在 `index.html` 文件中找到对应的视频标签（搜索 `videos/video1.mp4` 等示例路径）
3. 将 `src` 属性的值修改为您的视频文件名，例如：
   ```html
   <source src="videos/your-video-filename.mp4" type="video/mp4">
   ```
4. 确保视频格式为 MP4 格式，以获得最佳的浏览器兼容性
5. 同时更新作品的标题和描述

## 如何添加更多作品

如果您需要添加更多的作品，可以复制现有的作品项并进行修改：

1. 对于图片作品，复制以下代码块并修改：
   ```html
   <div class="portfolio-item images">
       <div class="portfolio-overlay">
           <h3>新作品标题</h3>
           <p>新作品描述</p>
       </div>
       <img src="images/new-work.jpg" alt="新作品">
   </div>
   ```

2. 对于视频作品，复制以下代码块并修改：
   ```html
   <div class="portfolio-item videos">
       <div class="portfolio-overlay">
           <h3>新视频标题</h3>
           <p>新视频描述</p>
       </div>
       <video controls>
           <source src="videos/new-video.mp4" type="video/mp4">
           您的浏览器不支持视频播放。
       </video>
   </div>
   ```

## 如何修改个人信息

1. 在 `index.html` 文件中找到 "关于我" 部分（搜索 `<section id="about"`）
2. 修改文本内容和个人照片
3. 在 "联系我" 部分（搜索 `<section id="contact"`）修改您的联系方式

## 最佳实践建议

1. **图片优化**：
   - 确保图片大小适中（建议每张图片不超过2MB）
   - 使用图片编辑工具压缩图片，如Photoshop、在线压缩工具等
   - 保持图片比例一致，建议使用16:9或4:3比例

2. **视频优化**：
   - 压缩视频文件，保持较小的文件大小（建议每个视频不超过20MB）
   - 使用MP4格式，确保良好的浏览器兼容性
   - 可以考虑使用视频缩略图提高加载速度

3. **内容更新**：
   - 定期更新作品，保持网站内容新鲜
   - 为每个作品添加清晰的标题和描述
   - 可以按类别或时间顺序组织作品

4. **网站维护**：
   - 定期检查网站链接是否正常
   - 确保图片和视频路径正确
   - 可以考虑添加社交媒体链接

## 预览网站

直接在浏览器中打开 `index.html` 文件即可查看网站效果。

## 部署网站

如果您想将网站发布到互联网上，可以：
1. 将所有文件上传到网站托管服务
2. 使用GitHub Pages等免费托管服务
3. 确保所有资源路径保持相对路径格式

祝您使用愉快！