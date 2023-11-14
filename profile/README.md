# 센서별 데이터 프로토콜

## 스트레인 게이지
12 bytes
```0x55, 0x55, timestamp(4 bytes), data(4 bytes), checksum(2 bytes)``` 

## Strain + IMU
18 bytes
```0x55, 0x55, timestamp(4 bytes), data(4 bytes), angle(6 bytes), checksum(2 bytes) ```

## 아날로그
12 bytes
```0x55, 0x55, timestamp(4 bytes), data(4 bytes), checksum(2 bytes)``` 

## 아날로그 3ch
8 bytes + 4 bytes * 설정에 따라 달라짐
```0x55, 0x55, timestamp(4 bytes), 1ch(4 bytes), 2ch(4 bytes), 3ch(4 bytes), checksum(2 bytes)``` 

## IMU
8 bytes + 6 bytes * 설정에 따라 달라짐
```0x55, 0x55, timestamp(4 bytes), acceleration(6 bytes), angular velocity(6 bytes), angle(6 bytes), checksum(2 bytes)``` 

## Noise analyizer
16 bytes
```0x55, 0x55, timestamp(4 bytes), booming(2 bytes), resonance(2 bytes), rumble(2 bytes), high freq(2 bytes), checksum(2 bytes)```

## Lidar
```0x55, 0x55, timestamp(4 bytes), data(4 bytes), checksum(2 bytes)```
