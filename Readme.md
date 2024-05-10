- Docker-image : la 1 file khong thay doi, chua src code va library... de ung dung chay, no giong snap

- Docker image giống như là khung xương định hình cho container, và sẽ tạo ra container khi thực hiện câu lệnh chạy image đó (image = class, còn container = instance nếu so sánh nó trong oop)

- container : là 1 run-time env mà ở đó người dùng có thể chạy ứng dụng độc lập

*image có thể không cần container còn container nhất định phải có ít nhất 1 image để chạy*


dockerfile----(build)-------> DOCKER_IMAGE----------(run)--------> DOCKER_CONTAINER