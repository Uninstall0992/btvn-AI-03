---
# try also 'default' to start simple
theme: apple-basic
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
image: https://www.eventus.si/en/iimg/7450/i.jpg
# some information about your slides (markdown enabled)
title: Bảng vẽ - bút vẽ
# apply UnoCSS classes to the current slide
layout: intro-image
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# duration of the presentation
preload: true
---

<div class="absolute top-10">
  <span class="font-700">
    25127542 - Đàm Anh Tuấn
  </span>
</div>

<div class="absolute bottom-10">
  <h1>Bảng vẽ - bút vẽ</h1>
  <p>Công cụ đắc lực của họa sĩ kĩ thuật số</p>
  <div @click="$slidev.nav.next" class="mt-12 py-1" hover:bg="white op-10">
  Nhấn Space để di chuyển đến trang tiếp theo. <carbon:arrow-right />
  </div>

</div>
<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
transition: slide-up
level: 2
---
# Di chuyển
## Phím tắt
|                                                     |                             |
| --------------------------------------------------- | --------------------------- |
| <kbd>right</kbd> / <kbd>space</kbd>                 | hoạt động hoặc slide tiếp theo     |
| <kbd>left</kbd>  / <kbd>shift</kbd><kbd>space</kbd> | hoạt động hoặc slide trước |
| <kbd>up</kbd>                                       | slide trước              |
| <kbd>down</kbd>                                     | slide tiếp theo                  |
| <kbd>enter</kbd>                                    | tự động chạy                |
| <kbd>esc</kbd>                                      | tắt tự động chạy            |
| <kbd>`</kbd>                                        | outline view                   |
<!-- https://sli.dev/guide/animations.html#click-animation -->

---
layout: two-cols
layoutClass: gap-16
---

# Mục lục


::right::

<Toc/>

---
transition: fade
layout: two-cols-header
---

# Khái niệm

Bảng vẽ kỹ thuật số là một thiết bị đầu vào chuyên dụng cho phép người dùng vẽ tay, tạo hình ảnh động và đồ họa một cách tự nhiên. Thiết bị này được thiết kế để mô phỏng trải nghiệm vẽ truyền thống bằng bút chì và giấy, nhưng mang lại nhiều tính năng và khả năng nâng cao hơn.
::left::
## Lịch sử phát triển
- **1950s**: Những thiết bị đầu vào đầu tiên được phát triển cho máy tính
- **1960s**: Bảng vẽ đầu tiên được phát triển bởi RAND Corporation
- **1980s**: Wacom giới thiệu công nghệ bút không dây, không pin
- **2000s**: Bảng vẽ màn hình LCD xuất hiện, cải thiện trải nghiệm người dùng
- **Hiện tại**: Tích hợp công nghệ cảm ứng đa điểm, áp lực, và nghiêng
::right::
## Ứng dụng chính
- Thiết kế đồ họa chuyên nghiệp
- Vẽ tranh kỹ thuật số
- Chỉnh sửa ảnh
- Hoạt hình và video
- Kiến trúc và thiết kế công nghiệp
- Giáo dục và đào tạo

[nguồn](https://www.webopedia.com/definitions/digitizing-tablet/)

---
image:
---

# Đặc điểm

## Bảng vẽ

<span>Bảng vẽ kỹ thuật có thể là một trong ba loại sau đây, mỗi loại mang theo những đặc điểm riêng biệt cuả nó</span> [nguồn](https://www.xp-pen.com/blog/types-of-drawing-tablets.html)

<div mt-6 />

<div grid grid-cols-3 gap-3 h-75>

<v-clicks>

<div border="2 solid white/5" rounded-lg overflow-hidden bg="white/5" backdrop-blur-sm h-full>
  <div flex items-center bg="white/10" backdrop-blur px-3 py-2 rounded-md>
    <div i-carbon:draw text-amber-300 text-sm mr-2 />
    <div font-semibold>
      Bảng vẽ đơn giản
    </div>
  </div>
  <div px-4 py-3>
    <div flex flex-col gap-3>
      <div>
        <div text-sm font-medium>Tấm vẽ đơn giản</div>
        <div text-xs opacity-70>Phải kết nối vào máy tính để sử dụng với bút</div>
      </div>
      <div>
        <div text-sm font-medium>Đòi hỏi kỹ năng</div>
        <div text-sm opacity-70>Người dùng vừa phải nhìn màn hình máy tính vừa phải chuyển động tay</div>
      </div>
      <div>
        <div text-sm font-medium>Giá thành thấp</div>
        <div text-xs opacity-70>Giao động phải chăng kể cả với bảng lớn</div>
      </div>
      <div>
        <div text-sm font-medium>Chống gù</div>
        <div text-xs opacity-70>Người dùng không cần cúi người xuống khi dùng như các loại có màn hình </div>
      </div>
    </div>
  </div>
</div>

<div border="2 solid white/5" rounded-lg overflow-hidden bg="white/5" backdrop-blur-sm h-full>
  <div flex items-center bg="white/10" backdrop-blur px-3 py-2 rounded-md>
    <div i-carbon:tablet-landscape text-blue-300 text-sm mr-2 />
    <div font-semibold>
      Bảng vẽ màn hình
    </div>
  </div>
  <div px-4 py-3>
    <div flex flex-col gap-3>
      <div>
        <div text-sm font-medium>Gắn màn hình</div>
        <div text-xs opacity-70>Người dùng vẽ trực tiếp lên bảng vẽ</div>
      </div>
      <div>
        <div text-sm font-medium>Giá thành cao</div>
        <div text-xs opacity-70>Có thể đắt bằng các máy tính, laptop tầm trung đặc biệt là với những màn hình lớn</div>
      </div>
    </div>
  </div>
</div>

<div border="2 solid white/5" rounded-lg overflow-hidden bg="white/5" backdrop-blur-sm h-full>
  <div flex items-center bg="white/10" backdrop-blur px-3 py-2 rounded-md>
    <div i-carbon:screen text-green-300 text-sm mr-2 />
    <div font-semibold>
      Bảng vẽ máy tính
    </div>
  </div>
  <div px-4 py-3>
    <div flex flex-col gap-3>
      <div>
        <div text-sm font-medium>Tích hợp máy tính</div>
        <div text-xs opacity-70>Không cần máy tính để chạy phần mềm vẽ</div>
      </div>
      <div>
        <div text-sm font-medium>Giá thành rất cao</div>
        <div text-xs opacity-70>Có thể đắt bằng các máy tính, laptop cao cấp</div>
      </div>
    </div>
  </div>
</div>

</v-clicks>

</div>

---
layout: 3-images
imageLeft: "https://www.zdnet.com/a/img/resize/a0b30b508195956bd9fcd92d5ff1572eaeb78cd4/2023/02/16/35775989-197a-43ce-8c97-13936dde5f4f/pxl-20230216-173948408.jpg?auto=webp&fit=crop&height=900&width=1200"
imageTopRight: "https://astropad.com/wp-content/uploads/2024/01/Wacom-Cintiq-16-.webp"
imageBottomRight: "https://store-img.huion.com.cn/3/a6c/standalone-tablet-mobile.webp"
---

---

## Bút cảm ứng
<span>Bút cảm ứng hoạt động theo hai nguyên lý căn bản: Điện dung và cộng hưởng điện từ. Hai nguyên lý này quyết định khả năng chuyển động của bút được nhận diện.</span> [nguồn](https://www.xp-pen.com/blog/can-any-stylus-work-on-any-drawing-tablet.html)

<div mt-6 grid grid-cols-2 gap-6>
  <div
    v-click
    border="2 solid red-800" bg="red-800/20"
    rounded-lg overflow-hidden
  >
    <div bg="red-800/40" px-4 py-2 flex items-center>
      <div i-carbon:touch-1 text-red-300 text-xl mr-2 />
      <span font-bold>Điện dung</span>
    </div>
    <div px-4 py-3 flex flex-col gap-2>
      <div flex items-center gap-2 py-1>
        <div i-carbon:fingerprint-recognition text-amber-300 text-xl />
        <div>
          <div font-bold>Nhái cú chạm con người</div>
          <div text-sm opacity-80>Dựa trên khả năng dẫn điện của ngón tay</div>
        </div>
      </div>
      <div flex items-center gap-2 py-1>
        <div i-carbon:machine-learning-model text-amber-300 text-xl />
        <div>
          <div font-bold>Tương thích cao</div>
          <div text-sm opacity-80>Phù hợp với nhiều thiết bị cảm ứng mới sử dụng công nghệ điện dung</div>
        </div>
      </div>
      <div flex items-center gap-2 py-1>
        <div i-carbon:user text-amber-300 text-xl />
        <div>
          <div font-bold>Dễ phối hợp</div>
          <div text-sm opacity-80>Thiết bị điện dung phân biệt được bàn tay và bút cảm ứng</div>
        </div>
      </div>
    </div>
  </div>

  <div
    v-click
    border="2 solid green-800" bg="green-800/20"
    rounded-lg overflow-hidden
  >
    <div bg="green-800/40" px-4 py-2 flex items-center>
      <div i-carbon:pen text-green-300 text-xl mr-2 />
      <span font-bold>Cộng hưởng điện từ</span>
    </div>
      <div bg="green-900/30" rounded-lg p-3 flex flex-col gap-2>
        <div font-bold text-sm>Chủ động</div>
        <div flex items-center gap-2>
          <div i-carbon:battery-full text-green-400 />
          <span text-sm>Sử dụng điện</span>
        </div>
        <div flex items-center gap-2>
          <div i-carbon:checkmark-outline text-green-400 />
          <span text-sm>Nhạy và chính xác</span>
        </div>
        <div flex items-center gap-2>
          <div i-carbon:hourglass text-green-400 />
          <span text-sm>Độ bền có hạn</span>
        </div>
        <div font-bold text-sm>Bị động</div>
        <div flex items-center gap-2>
          <div i-carbon:battery-charging text-green-400 />
          <span text-sm>Lấy năng lượng trực tiếp từ sóng điện từ của thiết bị vẽ</span>
        </div>
              <div bg="green-900/30" rounded-lg p-3 mt-1>
                <div font-bold text-sm mb-2>Thiết bị vẽ chuyên nghiệp thường hỗ trợ bút cộng hưởng điện từ</div>
        </div>
        </div>
    </div>

</div>

---


## Nguyên lý hoạt động

<div mt-6 />

<div grid grid-cols-2 gap-6>
  <div
    v-click="1"
    border="2 solid lime-800" bg="lime-800/20"
    rounded-lg overflow-hidden
    transition duration-500 ease-in-out
    :class="$clicks < 1 ? 'opacity-0 translate-y-20' : 'opacity-100 translate-y-0'"
  >
    <div bg="lime-800/40" px-4 py-4 flex items-center>
      <div> Cộng hưởng điện từ </div>
    </div>
```mermaid 
sequenceDiagram
    participant Bút
    participant Thiết bị
    Thiết bị ->> Bút: Trường điện từ biến thiên
    note over Bút,Thiết bị: Bút cảm ứng nhận được và phản hồi
    Bút->>Thiết bị: Sóng điện từ không liên tục
    note over Bút,Thiết bị: Thiết bị xác định được vị trí của bút
```
  </div>

  <div
    v-click="2"
    border="2 solid green-800" bg="green-800/20"
    rounded-lg overflow-hidden
    transition duration-500 ease-in-out
    :class="$clicks < 2 ? 'opacity-0 translate-y-20' : 'opacity-100 translate-y-0'"
  >
    <div bg="green-800/40" px-4 py-3 flex items-center>
      Điện dung
    </div>
```mermaid 
flowchart TD
    A[\Bút/]---|Thay đổi điện dung|B[\Màn hình/]
    B[\Màn hình/] ---|Báo cáo|C[\Thiết bị/]
```
  </div>
</div>



---
class: px-20
---

# Hiệu năng và Thông số kỹ thuật

<div mt-4 mb-4>
  <h2>Các yếu tố quan trọng cần xem xét khi chọn bảng vẽ</h2>
  <p>Để đảm bảo trải nghiệm vẽ tốt nhất và phù hợp với nhu cầu sử dụng, người dùng cần đặc biệt chú ý đến các thông số kỹ thuật sau:</p>
</div>

<div flex items-center gap-4>

<v-clicks>
  <div
    :class="$clicks < 1 ? 'translate-x--20 opacity-0' : 'translate-x-0 opacity-100'"
    rounded-lg
    border="2 solid yellow-800" bg="yellow-800/20"
    backdrop-blur
    flex-1 h-full
    transition duration-500 ease-in-out
  >
    <div px-2 py-12 flex items-center justify-center>
      <div i-carbon:area text-yellow-300 h-20 w-20 />
    </div>
    <div bg="yellow-800/30" w-full px-4 py-2 h="8rem" flex items-center justify-center text-center flex-col>
      <span class="font-bold mb-2">Diện tích vùng hoạt động</span>
      <span class="text-sm">Kích thước càng lớn càng cho phép thao tác chi tiết và thoải mái hơn</span>
    </div>
  </div>
  <div
    :class="$clicks < 2 ? 'translate-x--20 opacity-0' : 'translate-x-0 opacity-100'"
    rounded-lg
    border="2 solid lime-800" bg="lime-800/20"
    backdrop-blur
    flex-1 h-full
    transition duration-500 ease-in-out
  >
    <div px-2 py-12 flex items-center justify-center>
      <div i-carbon:pressure text-lime-300 h-20 w-20 />
    </div>
    <div bg="lime-800/30" w-full px-4 py-2 h="8rem" flex items-center justify-center text-center flex-col>
      <span class="font-bold mb-2">Độ nhạy áp lực</span>
      <span class="text-sm">Từ 2,048 trở lên, càng cao càng cho phép kiểm soát nét vẽ tốt hơn</span>
    </div>
  </div>
  <div
    :class="$clicks < 3 ? 'translate-x--20 opacity-0' : 'translate-x-0 opacity-100'"
    rounded-lg
    border="2 solid emerald-800" bg="emerald-800/20"
    backdrop-blur
    flex-1 h-full
    transition duration-500 ease-in-out
  >
    <div px-2 py-12 flex items-center justify-center>
      <div i-carbon:angle text-emerald-300 h-20 w-20 />
    </div>
    <div bg="emerald-800/30" w-full px-4 py-2 h="8rem" flex items-center justify-center text-center flex-col>
      <span class="font-bold mb-2">Hỗ trợ nghiêng bút</span>
      <span class="text-sm">Cho phép tạo hiệu ứng như vẽ bằng bút chì thật, hỗ trợ góc nghiêng lên đến 60 độ</span>
    </div>
  </div>
  <div
    :class="$clicks < 4 ? 'translate-x--20 opacity-0' : 'translate-x-0 opacity-100'"
    rounded-lg
    border="2 solid sky-800" bg="sky-800/20"
    backdrop-blur
    flex-1 h-full
    transition duration-500 ease-in-out
  >
    <div px-2 py-12 flex items-center justify-center>
      <div i-carbon:pen-fountain text-sky-300 h-20 w-20 />
    </div>
    <div bg="sky-800/30" w-full px-4 py-2 h="8rem" flex items-center justify-center text-center flex-col>
      <span class="font-bold mb-2">Chất lượng xây dựng</span>
      <span class="text-sm">Độ bền vật liệu, chất lượng bề mặt, và độ tin cậy của các nút bấm</span>
    </div>
  </div>
</v-clicks>

</div>

---

# Nhà sản xuất
[nguồn](https://drawingipad.com/best-drawing-tablet-brands-and-their-sites/)
<div flex justify-between items-center>
  <span w="1/2">Thương hiệu của bảng vẽ sẽ quyết định chất lượng và giá thành </span>
  <div i-carbon:cache text-7xl />
</div>

<div mt-6 grid grid-cols-3 gap-4>
  <div
    v-click
    border="2 solid indigo-800" bg="indigo-800/20"
    rounded-lg overflow-hidden
  >
    <div bg="indigo-800/40" px-4 py-2 flex items-center justify-center>
      <div  text-indigo-300 text-xl mr-2 />
      <span font-bold>1: Veikk</span>
    </div>
    <div px-3 py-3 flex flex-col gap-1>
      <div text-sm opacity-80>Thương hiệu Trung Quốc, thành lập 2009</div>
      <div flex items-center gap-1 text-xs>
        <div i-carbon:checkmark-outline text-green-400 />
        <span>Giá thành thấp</span>
      </div>
      <div flex items-center gap-1 text-xs>
        <div i-carbon:misuse-outline text-red-400 />
        <span>Ít ai biết đến</span>
      </div>
    </div>
  </div>

  <div
    v-click
    border="2 solid purple-800" bg="purple-800/20"
    rounded-lg overflow-hidden
  >
    <div bg="purple-800/40" px-4 py-2 flex items-center justify-center>
      <div  text-purple-300 text-xl mr-2 />
      <span font-bold>2: UGEE</span>
    </div>
    <div px-3 py-3 flex flex-col gap-1>
      <div text-sm opacity-80>Thương hiệu Trung Quốc, thành lập năm 1998</div>
      <div flex items-center gap-1 text-xs>
        <div i-carbon:checkmark-outline text-green-400 />
        <span>Giá thành thấp</span>
      </div>
      <div flex items-center gap-1 text-xs>
        <div i-carbon:checkmark-outline text-green-400 />
        <span>Có vài sản phẩm nổi bật</span>
      </div>
    </div>
  </div>

  <div
    v-click
    border="2 solid pink-800" bg="pink-800/20"
    rounded-lg overflow-hidden
  >
    <div bg="pink-800/40" px-4 py-2 flex items-center justify-center>
      <div  text-pink-300 text-xl mr-2 />
      <span font-bold>3: XPPEN</span>
    </div>
    <div px-3 py-3 flex flex-col gap-1>
      <div text-sm opacity-80>Thương hiệu Trung Quốc, thành lập Nhật Bản năm 2005</div>
      <div flex items-center gap-1 text-xs>
        <div i-carbon:checkmark-outline text-green-400 />
        <span>Giá thành trung bình</span>
      </div>
      <div flex items-center gap-1 text-xs>
        <div i-carbon:checkmark-outline text-green-400 />
        <span>Sản phẩm đa dạng</span>
      </div>
    </div>
  </div>
</div>

<div v-click mt-4 grid grid-cols-2 gap-4>
  <div bg="red-800/20" rounded-lg overflow-hidden>
    <div bg="red-800/40" px-4 py-2 flex items-center>
      <div  text-red-300 text-xl mr-2 />
      <span font-bold>Xencelabs</span>
    </div>
    <div px-4 py-3 flex flex-col gap-1>
      <div flex items-center justify-between>
        <div>Thương hiệu Trung Quốc cao cấp thành lập 2019</div>
      </div>
      <div flex items-center justify-between>
        <div>Đầy đủ tính năng, sáng tạo</div>
      </div>
    </div>
  </div>

  <div bg="green-800/20" rounded-lg overflow-hidden>
    <div bg="green-800/40" px-4 py-2 flex items-center>
      <div text-green-300 text-xl mr-2 />
      <span font-bold>Wacom</span>
    </div>
    <div px-4 py-3 flex flex-col gap-1>
      <div flex items-center justify-between>
        <div>Thương hiệu Nhật Bản thành lập 1983</div>
      </div>
      <div flex items-center justify-between>
        <div>Tiêu chuẩn vàng về bảng thiết kế đồ họa</div>
        <div text-green-400 font-bold flex items-center>
        </div>
      </div>
    </div>
  </div>
</div>

---
layout: image-left
image: https://cdn.mos.cms.futurecdn.net/KFpak7HK8HfdMHsMNW8ZpH-970-80.jpg.webp
---

# Sản phẩm
## Wacom Intuos Pro
### Giá: 7-14 triệu
### Thông số
- Diện tích: 187 x 105mm / 7.4 x4.1in
- Độ nhạy áp lực: 8,192 mức
- Kết nối: USB, Bluetooth
- Hỗ trợ hệ điều hành: Windows, macOS
### Lý do nên mua 
<ol>
<li>1. Chất lượng cao </li>
<li>2. Nhẹ và mỏng </li>
<li>3. Chính xác </li>
</ol>

### Lý do không nên mua 
<ol>
<li> Chỉ một bút cảm ứng </li>
</ol>

---
layout: image-right
image: https://cdn.mos.cms.futurecdn.net/DLTvVonSxtmE6Th4MzY7vh-970-80.jpg.webp
---

## Gói Xencelabs Pen Tablet Medium
### Giá: 10 triệu
### Thông số
- Diện tích: 261.6 x 147.2mm / 10.3 x 5.8in
- Độ nhạy áp lực: 8,192 mức
- Kết nối: USB, không dây
- Hỗ trợ hệ điều hành: Windows, macOS, Linux
### Lý do nên mua 
<ol>
<li>1. Không dây </li>
<li>2. Chất lượng cao </li>
<li>3. Trải nghiệm tốt </li>
</ol>

### Lý do không nên mua 
<ol>
<li> Thiếu nổi bật </li>
</ol>

---
layout: image-left
image: https://cdn.mos.cms.futurecdn.net/rLxhGGy8iqySYoB4ZZKwzL-970-80.jpg.webp
---

## Xencelabs Pen Display 16
### Giá: 33 triệu
### Thông số
- Diện tích: 342.9 x 196.7mm / 13.5 x 7.75in
- Độ nhạy áp lực: 8,192 mức
- Kết nối: USB, USB, HDMI, DisplayPort
- Hỗ trợ hệ điều hành: Windows, macOS, Linux
### Lý do nên mua 
<ol>
<li>1. Màn hình đẹp </li>
<li>2. Bút cảm ứng chất lượng cao </li>
<li>3. Thiết kế tốt </li>
</ol>

### Lý do không nên mua 
<ol>
<li> Thiếu nút nhấn </li>
</ol>

---
layout: image-right
image: https://cdn.mos.cms.futurecdn.net/mi4QfXBRgamjnCeSAyakH8-970-80.jpg.webp
---

## Ugee 16
### Giá: 6 triệu
### Thông số
- Diện tích: 263.2 x 148.1mm / 10.4 x 5.8in
- Độ nhạy áp lực: 16,348 mức
- Kết nối: USB
- Hỗ trợ hệ điều hành: Windows, macOS, ChromeOS, Harmony, Android
### Lý do nên mua 
<ol>
<li>1. Độ chính xác cao </li>
<li>2. Thiết kế thông minh </li>
<li>3. Rẻ </li>
</ol>

### Lý do không nên mua 
<ol>
<li> Không điều khiển được bằng chạm </li>
</ol>

---
layout: image-left
image: https://cdn.mos.cms.futurecdn.net/HfjEUJ8aXQd4KULemzhuv3-970-80.jpg.webp
---

## XP-Pen Magic Drawing Pad
### Giá: 13 triệu
### Thông số
- Diện tích: 203.2 x 127mm / 8 x 5in
- Độ nhạy áp lực: 16,348 mức
- Kết nối: USB, Bluetooth, Wifi
### Lý do nên mua 
<ol>
<li>1. Giá thành tốt </li>
<li>2. Nhẹ, dễ đem đi </li>
<li>3. Trải nghiệm tốt </li>
</ol>

### Lý do không nên mua 
<ol>
<li> Phản hồi không được nhạy </li>
</ol>

[Nguồn](https://www.creativebloq.com/features/best-drawing-tablet)

---

# AI


<div flex items-center justify-center gap-8>
  <div
    v-click="1"
    flex flex-col items-center
    transition duration-500 ease-in-out
    :class="$clicks < 1 ? 'opacity-0 scale-90' : 'opacity-100 scale-100'"
  >
    <div
      border="2 solid red-800" bg="red-800/20"
      rounded-lg p-6 w-100
    >
      <div flex items-center mb-4>
        <div i-carbon:share-knowledge text-red-300 text-2xl mr-2 />
        <span font-bold text-xl>Prompt</span>
      </div>
      <div bg="red-900/30" rounded-lg p-3 mb-3>
        <div flex items-center gap-2 mb-2>
          <div i-carbon:user text-red-300 />
          <span font-semibold>Tuấn</span>
        </div>
        <div text-sm space-y-1>
          <div flex items-center gap-1>
            <div/>
            <span text-xs>reformat the code for me</span>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div
    v-click="2"
    flex items-center
    transition duration-500 ease-in-out
    :class="$clicks < 2 ? 'opacity-0' : 'opacity-100'"
  >
    <div i-carbon:arrow-right text-4xl text-green-400 animate-pulse />
  </div>

  <div
    v-click="3"
    flex flex-col items-center
    transition duration-500 ease-in-out
    :class="$clicks < 3 ? 'opacity-0 scale-90' : 'opacity-100 scale-100'"
  >
    <div
      border="2 solid green-800" bg="green-800/20"
      rounded-lg p-6 w-100
    >
      <div flex items-center mb-4>
        <div i-carbon:bot text-green-300 text-2xl mr-2 />
        <span font-bold text-xl>AI</span>
      </div>
      <div bg="green-900/30" rounded-lg p-3 mb-3>
        <div flex items-center gap-2 mb-2>
          <div i-carbon:chat-bot text-green-300 />
          <span font-semibold>Claude Sonnet 3.5</span>
        </div>
        <div text-sm space-y-1>
          <div flex items-center gap-1>
            <div/>
            <span text-xs> The presentation should now be more consistent and professional-looking. Is there anything specific you'd like me to focus on or any other formatting improvements you'd like to see?
</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div
  v-click="3"
  mt-6 flex justify-center
  transition duration-500 ease-in-out
  :class="$clicks < 3 ? 'opacity-0' : 'opacity-100'"
>
  <div bg="blue-900/30" border="2 solid blue-800" rounded-lg px-5 py-3>
    <div flex items-center gap-3>
      <div i-carbon:analytics text-blue-300 text-2xl />
      <div>
        <div text-lg font-bold>Kết quả</div>
        <div text-sm>Sửa được hai lỗi chính tả. Phá nát một cái bảng.</div>
      </div>
    </div>
  </div>
</div>


---


<div flex items-center justify-center gap-8>
  <div
    v-click="1"
    flex flex-col items-center
    transition duration-500 ease-in-out
    :class="$clicks < 1 ? 'opacity-0 scale-90' : 'opacity-100 scale-100'"
  >
    <div
      border="2 solid red-800" bg="red-800/20"
      rounded-lg p-6 w-100
    >
      <div flex items-center mb-4>
        <div i-carbon:share-knowledge text-red-300 text-2xl mr-2 />
        <span font-bold text-xl>Prompt</span>
      </div>
      <div bg="red-900/30" rounded-lg p-3 mb-3>
        <div flex items-center gap-2 mb-2>
          <div i-carbon:user text-red-300 />
          <span font-semibold>Tuấn</span>
        </div>
        <div text-sm space-y-1>
          <div flex items-center gap-1>
            <div/>
            <span text-xs>rewrite my content for it to be longer</span>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div
    v-click="2"
    flex items-center
    transition duration-500 ease-in-out
    :class="$clicks < 2 ? 'opacity-0' : 'opacity-100'"
  >
    <div i-carbon:arrow-right text-4xl text-green-400 animate-pulse />
  </div>

  <div
    v-click="3"
    flex flex-col items-center
    transition duration-500 ease-in-out
    :class="$clicks < 3 ? 'opacity-0 scale-90' : 'opacity-100 scale-100'"
  >
    <div
      border="2 solid green-800" bg="green-800/20"
      rounded-lg p-6 w-100
    >
      <div flex items-center mb-4>
        <div i-carbon:bot text-green-300 text-2xl mr-2 />
        <span font-bold text-xl>AI</span>
      </div>
      <div bg="green-900/30" rounded-lg p-3 mb-3>
        <div flex items-center gap-2 mb-2>
          <div i-carbon:chat-bot text-green-300 />
          <span font-semibold>Claude Sonnet 3.5</span>
        </div>
        <div text-sm space-y-1>
          <div flex items-center gap-1>
            <div/>
            <span text-xs> I've made several significant enhancements to the content:
</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div
  v-click="3"
  mt-6 flex justify-center
  transition duration-500 ease-in-out
  :class="$clicks < 3 ? 'opacity-0' : 'opacity-100'"
>
  <div bg="blue-900/30" border="2 solid blue-800" rounded-lg px-5 py-3>
    <div flex items-center gap-3>
      <div i-carbon:analytics text-blue-300 text-2xl />
      <div>
        <div text-lg font-bold>Kết quả</div>
        <div text-sm>Thêm được vô số chi tiết Tuấn quá lười để làm. Tuy vậy, con AI không hiểu bố cục nên phá nát tận hai slide lận, khiến Tuấn phải đi sửa (nhưng không sửa cái bảng)</div>
      </div>
    </div>
  </div>
</div>

<div
  v-click="3"
  mt-6 flex justify-center
  transition duration-500 ease-in-out
  :class="$clicks < 3 ? 'opacity-0' : 'opacity-100'"
>
  <div bg="yellow-900/30" border="2 solid yellow-800" rounded-lg px-5 py-3>
    <div flex items-center gap-3>
      <div i-carbon:warning text-blue-300 text-2xl />
      <div>
        <div text-lg font-bold>Tổng kết</div>
        <div text-sm>Khác với sự gắn củn của Gemini và sự dài dòng của Mistral, Claude hỏi chi tiết rõ ràng từ người dùng không và hành động với sự cẩn trọng cao, như lập danh sách việc phải làm trước khi bắt đầu chỉnh sửa (tuy không tránh được hiều lầm).  À, với lại, cái script và widget tự chạy được viết bởi gia đình Gemini 2.5 (bao gồm flashlite, flash và pro) vì Tuấn không biết JavaScript.</div>
      </div>
    </div>
  </div>
</div>


---

## Kết luận & Tài liệu tham khảo

### Kết luận ngắn:
  - Nếu bạn là người mới: bắt đầu với bảng vẽ đơn hoặc model rẻ của XP-Pen/Veikk để làm quen.
  - Nếu bạn làm nghề: đầu tư vào Wacom hoặc Xencelabs (pen display hoặc standalone) để có trải nghiệm trực quan và độ bền.
  - Sử dụng AI để tăng tốc ý tưởng và tạo assets, nhưng luôn kiểm soát chất lượng và chú ý tới bản quyền.


### Tài liệu tham khảo:

- Webopedia — Digitizing tablet overview: https://www.webopedia.com/definitions/digitizing-tablet/
- XP-Pen blog — Types of drawing tablets: https://www.xp-pen.com/blog/types-of-drawing-tablets.html
- CreativeBloq — Best drawing tablets: https://www.creativebloq.com/features/best-drawing-tablet
- DrawingiPad — Brand comparison: https://drawingipad.com/best-drawing-tablet-brands-and-their-sites/

---

# Đánh giá mức độ hoàn thành 

| STT | Điểm | Kỹ năng PowerPoint |
|:-----|:------:|:------------------|
| 1 | 0.5 | Trang bìa (Tên nội dung, thông tin cá nhân) |
| 2 | 0.5 | Outline |
| 3 | 0.5 | Bullet & Numbering |
| 4 | 0.5 | Column |
| 5 | 0.5 | Insert picture/shape |
| 6 | 0.5 | Word Art/Smart Art |

---


| 7 | 0.5 | Action button |
| 8 | 0.5 | Footer (MSSV - Họ tên, Page number, Date) |
| 9 | 0.5 | Table |
| 10 | 0.5 | Animation |
| 11 | 0.5 | Transition |
| 12 | 0.5 | Diễn họa tự động |
| 13 | 0.5 | Trang cuối: Tài liệu tham khảo (Liên kết đối tượng ngoài) |
| 14 | 0.5 | Đánh giá mức độ hoàn thành |

---

| STT | Điểm | Kỹ năng sử dụng AI |
|:-----|:------:|:------------------|
| 1 | 2.0 | Sản phẩm AI |
| 2 | 1.0 | So sánh đánh giá, prompt |
