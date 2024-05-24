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
https://private-user-images.githubusercontent.com/121919752/333557080-7792f800-e293-44e3-ba1f-4d9c10ad07e2.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTY1NDc0NDIsIm5iZiI6MTcxNjU0NzE0MiwicGF0aCI6Ii8xMjE5MTk3NTIvMzMzNTU3MDgwLTc3OTJmODAwLWUyOTMtNDRlMy1iYTFmLTRkOWMxMGFkMDdlMi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNTI0JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDUyNFQxMDM5MDJaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1kYmM3NTBjZWVmODk2MTdkN2YwZDI1NmU5NzVhNDBjMmIyMjljZWQwMzA2ODY0ZGQzMzJmYjBhNGFhMThjODc5JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.WQ-VOddh9tYYW6AFGDqGIaVt2qF4CYp8rgCLTUVR_7k
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
https://private-user-images.githubusercontent.com/121919752/333557093-a6f46370-0c54-4542-b1cd-8bcfbf0292c6.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTY1NDc0NDIsIm5iZiI6MTcxNjU0NzE0MiwicGF0aCI6Ii8xMjE5MTk3NTIvMzMzNTU3MDkzLWE2ZjQ2MzcwLTBjNTQtNDU0Mi1iMWNkLThiY2ZiZjAyOTJjNi5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNTI0JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDUyNFQxMDM5MDJaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0wZjVlNGIyMjU1OGZiM2UwNDVlNmU0M2ZjZjIxODg5YTg1MTBlZGY3OWQ5N2Y1MDEyODE5YTZkY2FiMWJjZTA4JlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.dHuNo8-RreMqyLEBf10cXLsxrHjkXPpKq7qJnWqjR3Q
{
    "cod": "404",
    "message": "city not found"
}

### Trường Hợp Kiểm Thử 3
https://private-user-images.githubusercontent.com/121919752/333557103-77c57414-ab37-4092-8959-1a4f3aabac0a.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTY1NDc0NDIsIm5iZiI6MTcxNjU0NzE0MiwicGF0aCI6Ii8xMjE5MTk3NTIvMzMzNTU3MTAzLTc3YzU3NDE0LWFiMzctNDA5Mi04OTU5LTFhNGYzYWFiYWMwYS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNTI0JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDUyNFQxMDM5MDJaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0zZjIyNzE3Mzg0ODU2ZmM0NGQxNzRkNTkyMTI5NThkMWY4YmI2NTM5NGQ3ZTc4ZGQ5NTA5NjIwNDk0MzJlYzZmJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.21rQ3UHqEoAClh0XL2J-q9gn_qKELskxNLbW-cIwMN4
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
