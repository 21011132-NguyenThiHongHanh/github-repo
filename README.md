
Lấy hình ảnh
Để nhận được nhiều hơn 10 và các trường bổ sung, hãy đảm bảo sử dụng Khóa API của bạn từ email chào mừng làm tiêu đề hoặc tham số chuỗi truy vấn để truy cập tất cả hình ảnh và dữ liệu.'x-api-key'?api_key=

Có gì trong mảng hình ảnh

Mỗi chứa tệp hình ảnh, cùng với thông tin và thông tin của nó (nếu có), bất kỳ hoặc thông tin nào bạn tạo cũng sẽ được trả về.urlwidthheightbreedfavouritevote

Ví dụ về phản hồi (mảng các đối tượng hình ảnh)
[{
"id":"ebv",
"url":"https://cdn2.thecatapi.com/images/ebv.jpg",
"width":176,"height":540,
"breeds":[],
"favourite":{}
}]
Tham số truy vấn (chỉ được sử dụng với Khóa API hợp lệ)

Tên	kiểu  	sự miêu tả	                                             Mặc định

giới hạn	 1-100	                                         Số lượng hình ảnh để trả về giữa	1
trang	     0-n	                                           Số trang cần sử dụng khi Phân trang qua hình ảnh	0
trật tự	   ASC / DESC / RAND	                              Đơn đặt hàng trả lại hình ảnh trước ngày tải lên. RAND = random	RAND
has_breeds	1 hoặc 0	                                      Chỉ trả về hình ảnh có thông tin giống	0
breed_ids	  Chuỗi được phân tách bằng dấu phẩy	          ID của các giống để lọc hình ảnh. ví dụ: ?breed_ids=beng,abys	không ai
category_ids	Chuỗi được phân tách bằng dấu phẩy	        ID của các danh mục để lọc hình ảnh. ví dụ: ?breed_ids=1,5,14	không ai
sub_id	Xâu	Lọc hình ảnh có giá trị bạn đã sử dụng khi tải chúng lênsub_id	 không ai

Nhận được nhiều hơn 1 hình ảnh
Theo mặc định, chỉ có 1 hình ảnh được trả về. Để tăng điều này, hãy dùng tham số chuỗi truy vấnlimit

https://api.thecatapi.com/v1/images/search?limit=10
Lưu ý rằng có tối đa 10 mà không sử dụng Khóa API

Lấy một hình ảnh bằng ID
Bạn có thể truy xuất một Hình ảnh riêng lẻ bằng cách sử dụng ID duy nhất của Hình ảnh đó

URL yêu cầu mẫu

https://api.thecatapi.com/v1/images/0XYvRd7oD

Ví dụ về phản hồi

{
"id":"0XYvRd7oD",
"width":1204,"height":1445,
"url":"https://cdn2.thecatapi.com/images/0XYvRd7oD.jpg",
"breeds":[{
    "weight":{"imperial":"7  -  10","metric":"3 - 5"},
    "id":"abys","name":"Abyssinian",
    "temperament":"Active, Energetic, Independent, Intelligent, Gentle",
    "origin":"Egypt",
    "country_codes":"EG",
    "country_code":"EG",
    "life_span":"14 - 15",
    "wikipedia_url":"https://en.wikipedia.org/wiki/Abyssinian_(cat)"
}]
}
