# twoDifferent
// two different eqaul to target
int i = 0;
int j = 1;
int count = 0;
while (j < array.length) {
  if (array[j] - array[i] == target) {
    count++;
    j++;
  } else if (array[j] - array[i] > target) {
    i++;
  } else {
    j++;
  }
}
return count;


// array[j] - array[i] >  target
int i = 0;
int j = 0;
int count = 0;
while (j < array.length) {
  if (array[j] - array[i] <= target) {
    count += i;
    j++;
  } else {
    i++;
  }
}
return count; 
