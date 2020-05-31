# Conversion_of_Raster_data_to_vector_data
This MATLAB code would help to convert raster data (eg, maps) to vector data

C=[imread('1.bmp')];
%C=[1,2,3; 4,5,6; 7,8,9];
B=flip(C);
D=fliplr(B);
AAA=fliplr(D);
AV=[];
[r,c]=size(AAA);
for i = 1:r
    AV=[AV, AAA(i,:)];
end
length(AV);
A=AV'
