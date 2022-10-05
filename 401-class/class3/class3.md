# Beginners Guide to Big O
<ul>
<li>O(1) describes an algorithm that will always execute in the same time (or space) regardless of the size of the input data set.
</li>
<li>O(N) describes an algorithm whose performance will grow linearly and in direct proportion to the size of the input data set.</li>
<li>O(N²) represents an algorithm whose performance is directly proportional to the square of the size of the input data set.</li>
<li>O(2^N) denotes an algorithm whose growth doubles with each addition to the input data set. The growth curve of an O(2^N) function is exponential — starting off very shallow, then rising meteorically.</li>

</ul>

# Logarithms

## binary search
Binary search is a technique used to search sorted data sets. It works by selecting the middle element of the data set, essentially the median, and compares it against a target value. If the values match, it will return success. If the target value is higher than the value of the probe element, it will take the upper half of the data set and perform the same operation against it.<br>
This type of algorithm is described as O(log N). The iterative halving of data sets described in the binary search example produces a growth curve that peaks at the beginning and slowly flattens out as the size of the data sets increase e.g. an input data set containing 10 items takes one second to complete
