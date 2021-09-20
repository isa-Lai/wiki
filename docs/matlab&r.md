# MatLab $ R

## MatLab

using `disp` for print in matlab
useing `~` for any output not wanted, like `[~,maxlabidx] = max(t.Lab_sum); `

### Table
Read & Export table
```matlab
opts = detectImportOptions('course_grades_2021.xlsx');
opts = setvartype(opts,{'ID_Number','Name'},'string');
t = readtable('course_grades_2021.xlsx',opts);
```
Add new row or colume,use `size()` to check table size
```matlab
% add new colume
t.newcolumnnamd = dataadded;
t.Lab_sum = sum(t{:,3:6},2); % summing into new colume, note currently dont know why use 2 here. 2 is the dimention

% add new row
newrow(1,1).field1 = "isa";
newrow(1,1).field2 = "female";

Tnew = [Told;struct2table(newrow)];

%% or add directly using table
T1 = table('isa','female')
```

Query Table
```matlab
% filter
subtable = t(t.Name == "Isa-Lai",:); %condition
[maxlab,maxlabidx] = max(t.Lab_sum); %find max num and index
best_stu_lab = t(maxlabidx,:);
```

### Figure
Subplot using `nexttile` only support after R2019
```matlab
fig = figure('units', 'normalized', 'outerposition', [0, 0.08, 1, 0.9], 'Name',...
    'Question 1');
t = tiledlayout(1, 2);

nexttile; 
stem(n, q1a); grid on;
title("Question1a"); 
xlabel("n"); 
ylabel("x[n]");

nexttile;
stem(n, q1b); grid on;
title( "Question1b"); 
xlabel("n"); 
ylabel("x[n]");
title(t, "Isabelle Lai");
```
The old way writing subplot is using `subplot`
```matlab
fig = figure('Name','Question 1');
set(gcf,'WindowState','maximized'); set(0,'defaultAxesFontSize',20);
sgtitle('Isabelle Lai','FontSize',20);
xlim([-10 10]);

subplot(1,2,1)
stem(n,question1a); title('Question 1a'); 
xlabel('n'); ylabel('x[n]'); ylim([-1.5 1.5]);

subplot(1,2,2);
stem(n,question1b); title('Question 1b');
xlabel('n'); ylabel('x[n]'); ylim([-0.5 3.5]);
```
