# 사용할 기본 이미지
FROM rockylinux:8.8.20230518
ENV MY_TEST_ENV_CD 77777

# 패키지 업데이트 및 Nginx 설치
RUN dnf -y update && \
    dnf -y install epel-release && \
    dnf -y install nginx && \
    dnf clean all

# 필요한 포트 노출
EXPOSE 80

# Nginx를 포그라운드 모드로 실행
CMD ["nginx", "-g", "daemon off;"]