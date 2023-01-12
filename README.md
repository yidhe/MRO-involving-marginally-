clear;clc;
clear all
clf;
subplot(3,1,1)
y1=495:0.1:500;
T=500; r=5; l=5; 
d11=((y1-495)./(T-495)).^l;
plot(y1,d11,'b')
hold on
y1=495:0.1:500;  % 维度不一致，485 拆成485：495；
d12=((y1-485)./(T-485)).^l;
plot(y1,d12,'m')
hold on
fill ([y1,fliplr(y1)],[d11,fliplr(d12)],'c')
hold on
y0=485:0.1:495;  % 维度不一致，485 拆成485：495；
d02=((y0-485)./(T-485)).^l;
d01=((y0-y0)./(T-485)).^l;% d01=0;
plot(y0, d02,'m')
hold on
plot(y0, d01,'b')
hold on
fill ([y0,fliplr(y0)],[d01,fliplr(d02)],'c')
hold on

y2=500:0.1:510;
d21=((510-y2)./(510-T)).^r;
plot(y2,d21,'c')
hold on

% 添加辅助线；
y=484:0.1:511;
m1=0*y+1;
plot(y,m1,'k')
hold on
y=484:0.1:485;
m2=0*y+0;
plot(y,m2,'k')
y=510:0.1:511;
m3=0*y+0;
plot(y,m3,'k')
hold on
line([485 485],[0 1]);
hold on
line([500 500],[0 1]);
hold on
line([510 510],[0 1]);
hold on

subplot(3,1,2)
y1=495:0.1:500;
T=500; r=1; l=1; 
d11=((y1-495)./(T-495)).^l;
plot(y1,d11,'b')
hold on
y1=495:0.1:500;  % 维度不一致，485 拆成485：495；
d12=((y1-485)./(T-485)).^l;
plot(y1,d12,'m')
hold on
fill ([y1,fliplr(y1)],[d11,fliplr(d12)],'c')
hold on
y0=485:0.1:495;  % 维度不一致，485 拆成485：495；
d02=((y0-485)./(T-485)).^l;
d01=((y0-y0)./(T-485)).^l;% d01=0;
plot(y0, d02,'m')
hold on
plot(y0, d01,'b')
hold on
fill ([y0,fliplr(y0)],[d01,fliplr(d02)],'c')
hold on

y2=500:0.1:510;
d21=((510-y2)./(510-T)).^r;
plot(y2,d21,'c')
hold on

% 添加辅助线；
y=484:0.1:511;
m1=0*y+1;
plot(y,m1,'k')
hold on
y=484:0.1:485;
m2=0*y+0;
plot(y,m2,'k')
y=510:0.1:511;
m3=0*y+0;
plot(y,m3,'k')
hold on
line([485 485],[0 1]);
hold on
line([500 500],[0 1]);
hold on
line([510 510],[0 1]);
hold on

subplot(3,1,3)
y1=495:0.1:500;
T=500; r=0.5; l=0.5; 
d11=((y1-495)./(T-495)).^l;
plot(y1,d11,'b')
hold on
y1=495:0.1:500;  % 维度不一致，485 拆成485：495；
d12=((y1-485)./(T-485)).^l;
plot(y1,d12,'m')
hold on
fill ([y1,fliplr(y1)],[d11,fliplr(d12)],'c')
hold on
y0=485:0.1:495;  % 维度不一致，485 拆成485：495；
d02=((y0-485)./(T-485)).^l;
d01=((y0-y0)./(T-485)).^l;% d01=0;
plot(y0, d02,'m')
hold on
plot(y0, d01,'b')
hold on
fill ([y0,fliplr(y0)],[d01,fliplr(d02)],'c')
hold on

y2=500:0.1:510;
d21=((510-y2)./(510-T)).^r;
plot(y2,d21,'c')
hold on
% 添加辅助线；
y=484:0.1:511;
m1=0*y+1;
plot(y,m1,'k')
hold on
y=484:0.1:485;
m2=0*y+0;
plot(y,m2,'k')
y=510:0.1:511;
m3=0*y+0;
plot(y,m3,'k')
hold on
line([485 485],[0 1]);
hold on
line([500 500],[0 1]);
hold on
line([510 510],[0 1]);
hold on
