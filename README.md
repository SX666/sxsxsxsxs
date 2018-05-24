# sxsxsxsxs
Mystring Mystring::operator+(const Mystring&p1)const
{
    int len = p1.len + this.len;
    char* src = new char[len+1];
    strcpy(src,this.rep);
    strcat(src,p1.rep);
    Mystring mystr(src)
    delete [] src;
    return mystr;
}
const Mystring& Mystring::operator+=(const Mystring&p1)
{
    this->len += p1.len;
    cahr* src = this->rep;
    this->rep = new char*[len+1];
    strcpy(this->rep,src);
    strcat(this->rep,p1.rep);
    delete [] src;
    return *this;
}


