- Docker-image : la 1 file khong thay doi, chua src code va library... de ung dung chay, no giong snap

- Docker image giống như là khung xương định hình cho container, và sẽ tạo ra container khi thực hiện câu lệnh chạy image đó (image = class, còn container = instance nếu so sánh nó trong oop)

- container : là 1 run-time env mà ở đó người dùng có thể chạy ứng dụng độc lập

*image có thể không cần container còn container nhất định phải có ít nhất 1 image để chạy*


dockerfile----(build)-------> DOCKER_IMAGE----------(run)--------> DOCKER_CONTAINER

- Cau truc IMAGE
    FROM <he_dieu_hanh>
    COPY <file_can_chay> <destination>
    WORKDIR <path_de_vao_destination>
    CMD <lenh_de_chay_file>

- lenh build image : docker build -t <ten_tag_cua_image> <vi tri cua docker file (la dau "." neu dang o thu muc hien hanh)>

- lenh chay docker : docker run <ten_image>

- Ship image : docker tag <ten_image>:<tag_version_tuy_chon> <ten_repo_moi>:<version> *neu luc build image ko de version thi no se tu dong set thanh latest vi the version tuy chon luc ship se la latest*

- push image : docker push <ten_repo_moi_vua_tao>