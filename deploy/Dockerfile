# Используем базовый образ Ubuntu 22.04
FROM ubuntu:22.04

# Устанавливаем переменные среды для минимизации взаимодействий
ENV DEBIAN_FRONTEND=noninteractive

# Устанавливаем необходимые пакеты
RUN apt-get update && apt-get install -y \
    build-essential \        
    cmake \                  
    gdb \                    
    git \                    
    wget \                   
    clang \   
    && apt-get clean
    
# Устанавливаем рабочую директорию
WORKDIR /app

# Добавляем информацию о версии сборки (опционально)
LABEL maintainer="Andrey_claude_monet" \
      description="Образ для C++ разработки с использованием g++, CMake и Clang-Format" \
      version="1.0"
