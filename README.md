# strrev()
# chinese string rev function
# open mb_string 
function getRev($str, $encoding)
{
  $result = "";
  $len = mb_strlen($str);
  for($i=$len-1;$i>=0;$i--)
  {
    $result .= mb_substr($str,$i,1,$encoding);
  }
  return $result;
}
#echo getRev("hello_你");
