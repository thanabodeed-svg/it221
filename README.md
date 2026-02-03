name: ชื#อของ workflow
on: # Event ที#ทําให้ workflow ทํางาน
push:
branches: [ main ]
jobs:
build:
runs-on: ubuntu-latest # เลือกเครื#อง
steps: # Step ต่าง ๆ
- name: Checkout code
uses: actions/checkout@v4
- name: Run script
run: echo "Hello GitHub Actions"


