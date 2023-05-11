using System;

public class ExcelColumnConverter
{
    private string GetExcelColumnName(int columnNumber)
    {
        int dividend = columnNumber;
        string columnName = String.Empty;

        while (dividend > 0)
        {
            int modulo = (dividend - 1) % 26;
            columnName = Convert.ToChar(65 + modulo).ToString() + columnName;
            dividend = (dividend - modulo) / 26;
        }

        return columnName;
    }

    public static void Main(string[] args)
    {
        ExcelColumnConverter converter = new ExcelColumnConverter();
        
        // Example usage:
        int columnNumber = 27;
        string columnName = converter.GetExcelColumnName(columnNumber);
        Console.WriteLine("Column number " + columnNumber + " corresponds to Excel column " + columnName);
    }
}
