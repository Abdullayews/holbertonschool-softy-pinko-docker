FROM ubuntu:latest

RUN apt-get update
RUN apt-get upgrade -y

# Python3 və pip3 quraşdırılması
RUN apt-get install -y python3 python3-pip

# Əgər Ubuntu-da pip xətası olarsa qarşısını almaq üçün bu sətri əlavə edirik
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED

# Flask-ı pip3 ilə quraşdırırıq
RUN pip3 install flask

# İş qovluğunu təyin edirik və faylı kopyalayırıq
WORKDIR /app
COPY ./api.py /app/api.py

# Konteynir işə düşəndə Flask serverini başladırıq
CMD ["python3", "api.py"]
