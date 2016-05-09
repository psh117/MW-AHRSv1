# MW-AHRSv1
MoonWalker MW-AHRSv1 code
Product: http://www.devicemart.co.kr/1310790


## Structure

## How to use
  1. MW-AHRSv1.c와 MW-AHRSv1.h를 프로젝트에 포함시킵니다.
  2. 구조체 MW_AHRS를 선언하여 객체를 생성합니다.
  3. mw_ahrs_set_data_type, mw_ahrs_set_period를 호출하면 can_write_data에 써야 할 데이터가 저장됩니다.
  4. CAN Device로부터 받은 8바이트의 데이터는 can_read_data에 저장 후 mw_ahrs_input_data를 호출하면 데이터 처리가 되며 각 구조체 맴버를 업데이트 합니다.
