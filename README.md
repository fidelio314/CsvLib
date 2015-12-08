# CsvLib

Tools class for writing and reading csv files in PHP

# Write CSV

## example:
<pre><code>
//build the object
$writer = new CsvWriter();
//open a file path
$writer->open($lNameFile);
//write header array if needed
$header = ['test', 'test2'];
$writer->writeHeader($header);
//write row data
$writer->writeRow(array('data1', 'data2'));
$writer->__destruct();
</code></pre>


# Read CSV

## example:
<pre><code>
//build the object
$reader = new CsvReader();
//open a file path, define the delimiter if needed
$reader->open($lNameFile, ';');
//read line by line
while ($line = $reader->getRow()) {
 ...
}
$reader->__destruct();
</code></pre>
