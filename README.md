# CTDL-GT_linear_search_1.cpp
Tìm kiếm tuyến tính 
Nguồn tham khảo : https://xuixaicat.blogspot.com/2020/04/linear-search-tim-kiem-tuyen-tinh.html
Cài đặt: LinearSearch

void LinearSearch(int A[], int n, int x)
{
      int i;
      int dem = 0;
      for (i = 0; i < n; i++)
      {
            cout << "I = " << i << ": A[" << i << "] = " << A[i] << ", X = " << x << ". ";
            if (A[i] == x)
            {
                  cout << "Giong. Co X trong mang. Ket thuc." << endl;
                  //return i;
                  dem++;
                  break;

            }
            else if((A[i] != x) && (i < n -1))
            {
                  int t = i + 1;
                  cout << "Khac. Xem xet phan tu tiep theo A[" << t << "]" << endl;
                  dem++;
            }
      }
      if (dem == n-1)
      {
            cout << "Khac. Da xet den phan tu cuoi mang. Khong co X trong mang." << endl;
            dem++;
            //return -1;
      }
      cout << "So buoc so sanh " << dem << endl;
}
