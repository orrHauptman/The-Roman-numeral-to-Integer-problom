public static int RomanNumeralToInteger(string s)
{
    if (string.IsNullOrEmpty(s))
    {
        return 0;
    }
    int sum = 0;
    Dictionary<char, int> values = new Dictionary<char, int>();
    values['I'] = 1;
    values['V'] = 5;
    values['X'] = 10;
    values['L'] = 50;
    values['C'] = 100;
    values['D'] = 500;
    values['M'] = 1000;
    for (int i = 0; i < s.Length; i++)
    {
        int currentValue = values[s[i]];
        int nextValue = i < s.Length - 1 ? values[s[i + 1]] : 0;
        sum = currentValue<nextValue? sum-currentValue:sum+currentValue;
    }
    return sum;
}
