# CallTreeFormatter
vim call tree formatter

Format call tree 

    struct page *alloc_pages(gfp_t gfp_mask, unsigned int order)
              struct page *alloc_pages_current(gfp_t gfp, unsigned order) 
          
into below format,

    struct page *alloc_pages(gfp_t gfp_mask, unsigned int order)
              |
              |-> struct page *alloc_pages_current(gfp_t gfp, unsigned order) 
