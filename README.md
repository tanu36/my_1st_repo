# my_1st_repo
#rainfall_prediction_of_bihar_(1901_to_2017)
import matplotlib.pyplot as plt

years=list(range(1901,2017))
jan_mm=[51.8,4.6,5.3,6.3,16,14.4,1.3,14.7,7,2.4,9.4,5.5,0,0.2,8.2,0.6,2.7,0.6,40.2,0,26.8,12.2,1.3,2.5,7.7,16.3,24.4,41.2,51.6,11.6,1.3,0,28.3,30.1,21,7.7,0,12.4,5,0.9,16.2,34.4,34.7,27.3,50.7,0,5.6,11.1,16.5,9.8,7.3,1.1,29.7,12.5,20,19.3,75.2,16,81.2,1.4,11.7,13,3.4,1.4,0.4,21.2,0.2,29.1,5.2,22.1,17.3,12.9,22.9,3.9,9.1,2.3,5.3,13.4,23.4,4.7,31.3,4.4,13,128.6,8.8,1.1,0.7,1.2,8.9,0.3,14.5,2.6,9.4,28.3,6.8,26,10.5,8.4,0.1,0.5,1,13.4,22.7,13.9,0.1,0.2,25.6,0.3,0.1,4.2,18.1,5.1,17,12.8,9.3,0.7]
feb_mm=[19.6,0.7,4.7,1.7,30.1,56.9,55.2,38.6,6.3,4.8,0.1,8.5,38,22.7,57.1,16.5,19.7,0.1,7.7,19.2,0.6,4.6,35.1,12.7,1.8,0.6,36.4,21.5,1.1,7.6,32.4,8.2,13.1,13.7,19.6,6.9,66.3,17,42.3,43.8,2.8,43.5,16.9,32.6,24,21.3,5.6,7.5,42.8,11.8,1.5,10.3,4.2,8.4,6.7,4.7,2.8,2.7,1.5,0.1,35.8,7.8,1.7,3.3,1.2,6.9,0.1,1.7,9.3,13.4,14.6,38,10.2,0.7,4.1,12.4,2.9,27.8,19.4,2.4,5.7,6.1,1.7,33.9,0.5,13.9,3.7,15.3,8.7,30.26,3,3.1,4,29.1,11.6,21.7,1.1,11.2,0.2,12.1,0.5,11.3,39.7,2.1,14.3,0,34.2,4.4,0.4,1.1,7.7,2.7,22.6,33.5,1.8,0.6]
mar_mm=[2,3.5,32.6,8.6,39.4,6.1,0,6.6,2.2,23.9,18.1,8,22.5,0.3,7.9,1.8,3.8,31,6.5,0,1.5,1.8,7.7,29.7,31.9,0.1,11.4,13.6,11.4,0.5,0.7,3,0.6,4.6,0.8,0,11.3,65.5,0.7,14.7,0.2,42,0.2,42,1.4,5,10.2,3.6,5.7,22.1,5.8,20.1,8.7,0.8,2.3,9.6,11.6,4.7,9.4,42.7,1.4,9.5,9.4,2.4,15.7,0.1,38.6,7,9.7,3.2,5.1,2.7,3.8,21.9,12,0.9,1.3,16.8,2.3,9.5,14.3,28.2,8,1.3,0.5,5.4,27.3,6.9,13.8,7.9,0.1,24.5,1,2,0.2,2.9,23.6,0.4,3.6,3,2.2,10.2,2.2,12.1,1.9,25.4,3.2,1.1,0.2,9.2,7.3,0.6,8.4,27.2,5.6,22.8]
apr_mm=[17.3,4.7,5.3,21.4,0.9,27,2.2,72.8,5.7,13.1,25.4,1.4,29,6.4,25.3,5.8,29.5,11.6,2.6,21.2,9.6,13.5,8.8,52.9,12.8,3.1,18.3,16.2,6.6,1.6,14.8,62.1,9.1,0.7,7.7,10.7,2.9,1.7,5,4.6,18.2,40.7,34.1,32.4,52.3,7.5,11.3,35.5,2.2,8.2,24.6,16.7,0.6,11.9,5.3,0.5,26.4,18.6,5.2,2,20.8,17.5,21.9,7.1,0.9,30.6,3,20.7,17.9,91.4,3.2,4.4,9.9,11,8.9,17,24.5,21.3,7.9,47.9,14.7,45,11.2,8,16,37.7,46.9,0.2,14,8.9,2.6,24.5,7,0.1,3,29.3,26.6,3.8,37.2,12.6,25,21.9,32,7.7,19.2,20.3,10.4,2.9,6.5,23.9,20.4,32.3,0.7,38.7,3.9,21.8]
may_mm=[65.6,66.3,28.2,118.7,77.5,44.7,32.9,36.7,25.8,51.5,41.7,62.7,106.1,77,72.5,25.1,103.3,105.4,42.3,28.8,26.3,22,38.1,14.8,36.8,47,52.9,54.3,28.6,27.5,26.6,90.3,22,84.3,80,115.5,41.5,31.9,67.1,28.1,37,21.9,57.8,88.6,57.7,46.3,93.1,43.3,22.8,57,37.4,40.9,28.2,75.4,1.3,16.1,35.7,49.9,33.9,33.9,38.8,78.9,59.3,7.7,39.5,23.6,17.3,64.4,39.2,81.5,3.4,65,39.1,34.4,80.1,83.7,51.8,6.2,80.9,86.3,31,81.1,65.5,69.2,94.3,40.1,46.2,100.3,83.3,31.2,61.1,51.1,32.7,6.7,18.2,42.2,38.2,83.6,96.2,98.4,74.8,41.4,72.7,28.6,73.2,94.4,48.9,98.5,44.4,74.5,18.8,89.5,103.9,39.5,84,79.7]
jun_mm=[66.3,118.2,192.9,191.6,50.5,191.3,232.2,94,446,297.5,312.3,146.8,379.9,84.4,149.1,270.3,227.8,251.6,195,108.9,132.4,345.8,171.7,170.6,130.4,48.1,115.9,208,190.2,144.6,75.9,152.1,197,165.5,127.9,188.9,113.6,382.4,230.4,114.6,177.7,174.7,169.8,223.9,120.5,168.7,89.4,114.6,202.2,346.5,144.5,272.5,224.7,166.6,172.5,319.4,115.6,120.7,132.3,117.6,239.7,156.4,154,134.7,98.8,114.5,80.7,261.8,193.1,194.6,278,56.7,200.9,129.4,147.1,102.5,190.4,90.6,160.2,107.9,222.4,101.2,353.4,163.2,168.4,143.6,174.5,152.9,156.6,176.2,83.9,154.8,130.9,162.9,220.1,211,96.6,265.1,267.2,224.4,116.6,230.9,246.8,82.5,200,170.4,291.2,67.7,80.9,211,96.2,183.3,115.2,122.1,128.7,84.6]
jul_mm=[492.1,245.9,361,115,394.4,409.1,366.2,282.4,202.3,256.2,365.1,362.4,258.8,269.1,321.3,445.6,328.7,240.3,417.8,361.6,303.8,427.3,253.9,514,322.9,451.5,377.2,328.8,298.2,441.3,164.3,377.3,423.6,193.8,462.2,217.9,362.1,315,317.6,248.8,253.5,296,253.3,226.9,354.7,394.4,409,341.7,257,307.8,212.5,431.8,366.1,505.7,200.6,334.5,222.8,245.8,357.4,211.6,244.3,375.4,453.6,302.2,155.5,278.2,329.6,348.4,284.2,307,163.4,185.1,451.6,403.1,221,375.5,313.6,435.5,389.9,580.1,227.2,355.8,476.4,481.5,395.7,452,364.5,446,485.5,179.7,284.8,209.1,217.7,227.5,238.5,463.9,465.1,380.8,264.3,224.7,386.1,356.8,418.4,300,290.7,549.4,397.2,213.6,191.2,241.1,354,182,265.4,231.5,356.4,379.9]
aug_mm=[319.4, 225.5, 342.6, 351.3, 495.3, 430.1, 242.2, 167.3, 352.4, 328.8, 425.5, 302.9, 363, 460.4,415, 325.2, 249.3, 519.2, 228.5, 422, 363.5, 243.2, 295.7, 331.5, 276, 242.7, 272.9, 326.3, 247.8, 218.8, 249.3, 377.8, 251.3, 481.7, 261.5, 441.8, 385.1, 277.1, 314.9, 466, 330.4, 322.1, 322.8, 265.6, 267.8, 244.6, 329.8, 386.5, 313.3, 204.5, 291.9, 263.3, 308.6, 268.7, 286.3, 295.8, 451.1, 264.2, 285.5, 317.5, 395.4, 273.5, 157.7, 328.3, 308.3, 282.1, 293.1, 379.4, 235.6, 367.9, 154.9, 258.9, 317.5, 155.2, 292.8, 266, 252.6, 166.1, 375.3, 311.3, 164.5, 195.8, 216.9, 238, 263.5,539.8, 459.4, 171.9, 204.4, 324.2, 219.2, 357.3, 257.6, 335.7, 350.9, 287.6, 377.4, 347.5, 201.4, 225.9, 247.7, 310.6, 175.9, 309.1, 160.4, 340.6, 278.1, 298.9, 158.4, 278.7, 240.4, 213.6, 307.6, 287, 150.8, 342.8]
sept_mm=[155.1, 358.7, 173.9, 84.4, 353.9, 118.7, 149.9, 175.4, 258.5, 279.1, 104.7, 270.3, 98.4, 185.1, 265.2, 272.1, 254.4, 244.8, 337.6, 295.8, 241.3, 148.9, 320.3, 269.4, 211.6, 231.4, 83.3, 124.7, 290.9, 248.2, 191.2, 167.8, 231.2, 370.3, 449.2, 179.3, 201.4, 262, 171.6, 190.2, 347.2, 215.4, 221.3, 305.5, 271.8, 215.3, 248.9, 217.9, 113.4, 114.3, 297.7, 342.2, 129.5, 192.2, 359.8, 115.2, 224.2, 157.1, 348.1, 157.5, 216.3, 255.7, 219, 215, 83.1, 253.8, 79.2, 219.1, 229.5, 129.2, 209.7, 271.4, 229.2, 245.3, 372.6, 121, 248.6, 113, 190.5, 168.8, 170.5, 220.6, 219, 289, 221.1, 379.7, 153.2, 330.9, 201.2, 270.5, 85.9, 320, 226.5, 279.1, 162.5, 185.8, 188, 199.6, 314.8, 274.8, 192.8, 183.9, 115.3, 105.1, 285.2, 309, 117.1, 127.6, 105.7, 234.1, 233.8, 143.3, 160.3, 101.7, 357.9, 129.6]
oct_mm=[8.3, 28.5, 147, 98.1, 11.6, 32.9, 25.4, 43.1, 73.8, 61, 122.8, 14, 10.1, 75.3, 130.1, 116.5, 8.6, 58.6, 5.6, 37, 15.7, 74.4, 53.1, 17.6, 17.6, 21.5, 164.3, 231.4, 30.4, 76.1, 32.4, 77.6, 55.2, 2.6, 88.8, 194.6, 27.1, 56.9, 4.9, 47.8, 7, 37, 48.5, 154.8, 148.7, 61.5, 81, 103.4, 3, 28.7, 15.4, 18.4, 15.1, 35.7, 168.8, 11.6, 81.5, 233.8, 37.9, 236, 72.5, 138.7, 66.3, 22.2, 18.3, 10.3, 113.3, 15.3, 34.5, 138.6, 48.4, 158.2, 28, 51.7, 22.4, 147.1, 142.8, 88.5, 29.5, 1, 42.1, 69.9, 15.4, 188, 124.2, 52.8, 33.7, 28.2, 49.7, 7.2, 52.4, 34.3, 32.9, 11.4, 66.2, 27.8, 83, 114.1, 9.6, 181.3, 33.8, 142, 56.4, 34.3, 17.6, 39.6, 21.4, 72.6, 33.6, 10, 34.3, 197.1, 47.8, 10.4, 60.8, 50.1]
nov_mm=[7.3, 1.1, 0.1, 10.6, 0, 0.4, 0, 0, 0, 21.7, 17.8, 72.6, 0, 36.7, 0.4, 0, 0.1, 0, 0, 0, 0.7, 0.7, 61.7, 11, 1.8, 38.6, 0.9, 0, 24, 11.2, 78.7, 0.3, 9.8, 0.1, 0.4, 0.3, 0.8, 0, 0, 1.1, 0, 0, 0.2, 0, 14.9, 0.1, 36.2, 1.1, 0.1, 4.7, 3.4, 0.9, 0.2, 0.3, 36, 0, 0.7, 0, 2, 0.8, 0, 17.8, 2.7, 1.8, 17.1, 0.1, 0, 23.6, 0.4, 1.9, 24.6, 8.3, 0.3, 0, 0.7, 8.1, 4.8, 25.2, 0.2, 6.1, 21.5, 0, 1.5, 1.2, 1.3, 2.7, 1.5, 1, 0, 0, 1.4, 19.3, 4.4, 44.4, 0, 11, 14.5, 6.9, 0, 0.5, 1.4, 0.2, 3.1, 0, 2.9, 9.1, 0.1, 5.1, 5, 2, 6.4, 0.4, 0, 0, 0, 0]
dec_mm=[0.1, 0, 0, 3.8, 0.6, 0, 2.1, 0.3, 5.6, 0, 0, 0, 32.8, 0.6, 0, 0.2, 0, 0.7, 0, 0, 6.5, 0.4, 0.2, 0, 8.7, 0.2, 7.6, 44.4, 10.4, 0.7, 8.9, 0.3, 2.8, 0.1, 10.3, 1.1, 0, 0, 17.5, 0, 0.9, 0, 0.8, 3.2, 0, 0.3, 0, 0, 2.1, 0.1, 0.4, 0.8, 1.3, 0.1, 8.1, 2.7, 0.6, 0.1, 0, 10.1, 3.2, 0.2, 0, 2.4, 1.6, 1.5, 4.9, 0.3, 0, 0, 0, 0, 3.7, 0, 0.5, 17.3, 3.7, 10.3, 1, 3.9, 1, 14.1, 3, 7.1, 22.1, 2.3, 13.8, 14, 0.2, 19.2, 0.4, 0.1, 1.2, 23.8, 0, 30.6, 0, 0.6, 0.1, 0, 0.7, 3, 0, 0.2, 1.6, 7.5, 0, 0.8, 2.1, 0.9, 0, 0, 1.2, 0, 0, 0]
plt.title("Rainfall pridiction in bihar between 1901 and 2017")
plt.xlabel("year")
plt.ylabel("in MMs")
plt.xticks(rotation=90)
plt.plot(years,jan_mm,color="b")
plt.plot(years,feb_mm,color="r")
plt.plot(years,mar_mm,color="g")
plt.plot(years,apr_mm,color="m")
plt.plot(years,may_mm,color="y",ls=":")
plt.plot(years,jun_mm,color="g",ls="-.")
plt.plot(years,jul_mm,color="y",ls=":")
plt.plot(years,aug_mm,color="k")
plt.plot(years,sept_mm,color="c")
plt.plot(years,oct_mm,color="r",ls="--")
plt.plot(years,nov_mm,color="c")
plt.plot(years,dec_mm,color="m",ls="--")
plt.show()
