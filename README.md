# Kiểm thử API với Postman

## Giới thiệu
Mục tiêu của bài tập này là thực hành kiểm thử API bằng cách sử dụng Postman. Bài tập bao gồm các bước từ việc lựa chọn một API kiểm thử, phân tích tài liệu API, viết các trường hợp kiểm thử, thực hiện kiểm thử và ghi lại kết quả kiểm thử.

## API Được Chọn
API được lựa chọn cho bài tập này là **Random Data API**, một API phổ biến cung cấp dữ liệu cho người dùng.

## Thực Hiện Các Trường Hợp Kiểm Thử với Postman

### Trường Hợp Kiểm Thử 1: 
- **Điểm cuối**: `https://random-data-api.com/api/v2/users`
- **Phương thức**: GET


### Trường Hợp Kiểm Thử 2: 
- **Điểm cuối**: `https://random-data-api.com/api/v2/beers`
- **Phương thức**: GET


### Trường Hợp Kiểm Thử 3: 
- **Điểm cuối**: `https://random-data-api.com/api/v2/beers?beerType=light`
- **Phương thức**: GET



## Kết Quả Kiểm Thử

### Trường Hợp Kiểm Thử 1
![image](https://github.com/hoanvukhai/api-testing-with-postman/assets/129703780/cd21e27a-07c4-441c-b6f6-7f6f19bc7c70)
{
    "coord": {
        "lon": 105.8412,
        "lat": 21.0245
    },
    "weather": [
        {
            "id": 804,
            "main": "Clouds",
            "description": "overcast clouds",
            "icon": "04d"
        }
    ],
    "base": "stations",
    "main": {
        "temp": 306.15,
        "feels_like": 313.15,
        "temp_min": 306.15,
        "temp_max": 306.15,
        "pressure": 1004,
        "humidity": 64,
        "sea_level": 1004,
        "grnd_level": 1003
    },
    "visibility": 10000,
    "wind": {
        "speed": 4.26,
        "deg": 146,
        "gust": 6.97
    },
    "clouds": {
        "all": 95
    },
    "dt": 1716544748,
    "sys": {
        "type": 1,
        "id": 9308,
        "country": "VN",
        "sunrise": 1716502573,
        "sunset": 1716550264
    },
    "timezone": 25200,
    "id": 1581130,
    "name": "Hanoi",
    "cod": 200
}

### Trường Hợp Kiểm Thử 2
![image](https://github.com/hoanvukhai/api-testing-with-postman/assets/129703780/cb3508c4-5649-4e30-b913-ea75dde87fdd)
{
    "cod": "404",
    "message": "city not found"
}

### Trường Hợp Kiểm Thử 3
![image](https://github.com/hoanvukhai/api-testing-with-postman/assets/129703780/f52acd45-8aa7-4d67-8ab7-3d899cdc88af)
![image](https://github.com/hoanvukhai/api-testing-with-postman/assets/129703780/d1f3fab2-8489-494f-9f6d-c46df17d1710)
{
    "cod": 401,
    "message": "Invalid API key. Please see https://openweathermap.org/faq#error401 for more info."
}

## Báo Cáo Kiểm Thử Chi Tiết

**Mục Tiêu Kiểm Thử:**
- Xác định và xác thực các phản hồi của Random Data API dựa trên các truy vấn khác nhau.


**Kết Quả Kiểm Thử:**
- Tất cả các trường hợp kiểm thử được thực hiện và kết quả phù hợp với mong đợi.

**Khuyến Nghị:**
- API hoạt động tốt 
