# Real-Estate-Banking-Mortgage-Price-Prediction
A statistical model needs to be created to predict the potential demand in dollars amount of loan for each of the region in the USA. Also, there is a need to create a dashboard which would refresh periodically post data retrieval from the agencies.

# GIẢI THÍCH DỮ LIỆU:
I.THÔNG TIN VỀ ĐỊA LÝ:

UID: Mã định danh duy nhất cho mỗi bản ghi hoặc đơn vị (unique identifier).

BLOCKID: Mã định danh cho một khu vực dân cư cụ thể

SUMLEVEL: Cấp độ tóm tắt của dữ liệu (summary level), cho biết mức độ chi tiết của dữ liệu

COUNTYID: Mã định danh cho quận (county)

STATEID: Mã định danh của bang (state).

state: Tên của bang

state_ab: Tên viết tắt của bang (ví dụ: CA cho California, TX cho Texas).

city: Tên thành phố nơi dữ liệu được thu thập.

place: Tên địa điểm hoặc khu vực cụ thể

type: Loại hình khu vực (ví dụ: khu dân cư, khu thương mại...).

primary: Biểu thị một đơn vị chính trong dữ liệu hoặc vùng chính được nghiên cứu.

zip_code: Mã bưu điện của khu vực.

area_code: Mã vùng điện thoại cho khu vực đó.

lat vs lng: Vĩ độ và Kinh độ của vị trí

ALand: Diện tích đất tự nhiên (không bao gồm diện tích mặt nước) trong khu vực.

AWater: Diện tích mặt nước trong khu vực.

--------------------------------------------------------------------------------------------------------------------------------------------------------------

II.THÔNG TIN VỀ DÂN SỐ:

pop: Tổng dân số trong khu vực.

male_pop vs female_pop: Dân số nam giới và nữ giới

--------------------------------------------------------------------------------------------------------------------------------------------------------------

III.THÔNG TIN VỀ GIÁ NHÀ

rent_mean: Giá thuê nhà trung bình trong khu vực.

rent_median: Giá thuê nhà trung vị (median rent)

rent_stdev: Độ lệch chuẩn của giá thuê nhà, cho biết mức độ biến động của giá thuê.

rent_sample_weight: Trọng số mẫu dùng để tính toán các giá trị thuê nhà.

rent_samples: Số lượng mẫu thu thập cho giá thuê.

rent_gt_10, 15, 20, 25, 30, 35, 40, 50: Số lượng các hộ gia đình có tỷ lệ chi tiêu cho tiền thuê nhà trên 10, 15, 20, 25, 30, 35, 40, 50% thu nhập.

--------------------------------------------------------------------------------------------------------------------------------------------------------------

IV.THÔNG TIN VỀ THU NHẬP

hi_mean: Thu nhập hộ gia đình trung bình.

hi_median: Thu nhập hộ gia đình trung vị.

hi_stdev: Độ lệch chuẩn của thu nhập hộ gia đình.

hi_sample_weight: Trọng số mẫu dùng để tính thu nhập.

hi_samples: Số mẫu được sử dụng để tính toán thu nhập.

--------------------------------------------------------------------------------------------------------------------------------------------------------------

V.THÔNG TIN VỀ HỘ GIA ĐÌNH

family_mean: Thu nhập trung bình của hộ gia đình.

family_median: Thu nhập trung vị của hộ gia đình.

family_stdev: Độ lệch chuẩn của thu nhập hộ gia đình.

family_sample_weight: Trọng số mẫu cho thu nhập hộ gia đình.

family_samples: Số mẫu thu thập về thu nhập hộ gia đình.

pct_own: Tỷ lệ phần trăm các hộ gia đình sở hữu nhà.

--------------------------------------------------------------------------------------------------------------------------------------------------------------

VI.THÔNG TIN VỀ CHI PHÍ THẾ CHẤP

hc_mortgage_mean: Chi phí trung bình của khoản thế chấp nhà (mortgage cost).

hc_mortgage_median: Chi phí trung vị của khoản thế chấp.

hc_mortgage_stdev: Độ lệch chuẩn của chi phí thế chấp.

hc_mortgage_sample_weight: Trọng số mẫu cho các khoản thế chấp.

hc_mortgage_samples: Số mẫu thu thập về thế chấp.

--------------------------------------------------------------------------------------------------------------------------------------------------------------

VII.THÔNG TIN VỀ CHỦ SỞ HỮU VÀ NỢ

home_equity_second_mortgage: Giá trị tài sản nhà khi có thế chấp thứ hai

second_mortgage: Thông tin về khoản thế chấp thứ hai.

home_equity: Giá trị tài sản nhà (home equity) của chủ sở hữu.

debt: Tổng số nợ của chủ nhà.

second_mortgage_cdf, home_equity_cdf, debt_cdf: Phân phối tích lũy của các giá trị tương ứng.

--------------------------------------------------------------------------------------------------------------------------------------------------------------

VIII.TRÌNH ĐỘ HỌC VẤN

hs_degree: Tỷ lệ dân số có bằng trung học (high school degree).

hs_degree_male: Tỷ lệ nam giới có bằng trung học.

hs_degree_female: Tỷ lệ nữ giới có bằng trung học.

--------------------------------------------------------------------------------------------------------------------------------------------------------------

IX.THÔNG TIN CÁ NHÂN married: Tỷ lệ dân số đã kết hôn.

married_snp: Số người kết hôn không tính số người sống độc thân (single and never married population).

separated: Tỷ lệ dân số đã ly thân.

divorced: Tỷ lệ dân số đã ly dị.

male_age_mean: Tuổi trung bình của nam giới.

male_age_median: Tuổi trung vị của nam giới.

male_age_stdev: Độ lệch chuẩn tuổi của nam giới.

male_age_sample_weight, male_age_samples: Trọng số và số mẫu cho dữ liệu tuổi của nam giới.

female_age_mean: Tuổi trung bình của nữ giới.

female_age_median: Tuổi trung vị của nữ giới.

female_age_stdev: Độ lệch chuẩn tuổi của nữ giới.

female_age_sample_weight, female_age_samples: Trọng số và số mẫu cho dữ liệu tuổi của nữ giới.
